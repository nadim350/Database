# Database
# Week 3

### Assignment: Single Table Queries

### Question 1
Select * from goal;

![Screenshot (13)](https://github.com/user-attachments/assets/b827f996-bd0d-4139-a103-daa2a1551d73)


### Question 2
Select name, type from airport where iso_country = 'FI';

![Screenshot (14)](https://github.com/user-attachments/assets/fc8413a7-4c8f-4d8d-b1eb-38cbec2643cc)


### Question 3
select name from airport where iso_country = "FI" order by name;
![Screenshot (15)](https://github.com/user-attachments/assets/68734681-da9c-4789-8998-da6a1f8eb84e)



### Question 4
select name, type from airport where iso_country = "FI" order by type,name;

![Screenshot (16)](https://github.com/user-attachments/assets/1fac749b-1713-4aa2-9e8e-45b85a214ffb)


### Question 5
select name from country where name like "F%";
![Screenshot (17)](https://github.com/user-attachments/assets/59dea55b-1419-4eb4-9e29-7ffcf2b798f2)

### Question 6
select name from country where name like "%F%";
![Screenshot (18)](https://github.com/user-attachments/assets/5c775837-6a5f-4551-b06d-a1320d0e1e31)

### Question 7
select location from game where screen_name = "Vesa";
![Screenshot (19)](https://github.com/user-attachments/assets/5d218cd2-6501-48e6-9c6a-fcbbd01d2e06)


### Question 8
select co2_consumed from game where screen_name = "Ilkka";
![Screenshot (20)](https://github.com/user-attachments/assets/d4d518dc-f4f0-489c-b0c9-f6b2d6d65c61)



### Question 9
select distinct co2_budget from game;
![Screenshot (21)](https://github.com/user-attachments/assets/493a9147-247b-4d3a-ba12-6d5de13fd367)


### Question 10
SELECT 
    screen_name,
    co2_budget,
    co2_consumed,
    (co2_budget - co2_consumed) AS co2_left
FROM
    game
WHERE
    screen_name = 'Ilkka';

![Screenshot (22)](https://github.com/user-attachments/assets/fd437e55-7729-42b1-b6ad-edfdb8a28edf)


