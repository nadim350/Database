# Week 5

### Assignment: Aggregate Queries

### Question 1
select max(elevation_ft) from airport;

![Screenshot (43)](https://github.com/user-attachments/assets/04c7d636-c40d-45ff-9dc1-10ec4c830eec)

### Question 2
Select continent, count(*) from country group by continent;

![Screenshot (44)](https://github.com/user-attachments/assets/50e0f491-2db2-49c2-bcaf-3faee642f2cf)

### Question 3
select screen_name, count (*) from game, goal_reached where id = game_id group by screen_name;

![Screenshot (45)](https://github.com/user-attachments/assets/7352cb0c-12f3-4fe1-a240-669ca262dac3)


### Question 4
select screen_name from game where co2_consumed in(select min(co2_consumed) from game);

![Screenshot (47)](https://github.com/user-attachments/assets/274e03ce-3808-4907-b524-bef5008b4fd0)


### Question 5
select country.name, count(*) from airport, country where airport.iso_country = country.iso_country
group by country.iso_country
order by count(*) desc
limit 50;

Error !

### Question 6
select country.name
from airport, country
where airport.iso_country = country.iso_country
group by country.iso_country
having count(*) > 1000;

![Screenshot (48)](https://github.com/user-attachments/assets/16c0d6fd-3385-450f-b070-01238e66e292)

### Question 7
select name from airport where elevation_ft in (select max(elevation_ft) from airport);

![Screenshot (49)](https://github.com/user-attachments/assets/603a7e1f-b4f6-4781-8e7b-11628417fb71)


### Question 8 
select name from country where iso_country in (select iso_country from airport where elevation_ft in(
select max(elevation_ft) from airport));

![Screenshot (50)](https://github.com/user-attachments/assets/f2da5a62-e35b-45a3-8879-2bf09e5f843c)


### Question 9
select count(*) from game, goal_reached where id = game_id and screen_name = "Vesa" group by screen_name;

![Screenshot (51)](https://github.com/user-attachments/assets/d5d2dab0-82ed-4590-a866-4fede2cb061b)


### Question 10
select name from airport where latitude_deg in(select min(latitude_deg)
from airport);

![Screenshot (52)](https://github.com/user-attachments/assets/63a9db57-4523-4b97-8edc-b1c313a0839b)


