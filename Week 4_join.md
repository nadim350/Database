# Week 4

### Assignment: Join

### Question 1
Select country.name as "country name", airport.name as "airport name" 
from country join airport on country.iso_country = airport.iso_country where country.name = "Finland";

![Screenshot (33)](https://github.com/user-attachments/assets/fce21b64-af56-4b7e-b717-580383f4a848)


### Question 2
select screen_name, airport.name from game inner join airport on location = ident;

![Screenshot (34)](https://github.com/user-attachments/assets/05b0bd1e-6be6-4f01-b289-122bb36d78e9)


### Question 3
select screen_name, country.name from game inner join airport on location = ident;
inner join country on airport.iso_country = country.iso_country



### Question 4
select airport.name, screen_name from airport left join game on ident = location where airport.name like "%Hels%";

![Screenshot (35)](https://github.com/user-attachments/assets/665dd69b-baea-4a45-a709-e440f549b89f)


### Question 5
select name, screen_name from goal left join goal_reached on goal.id = goal_id left join game on game.id = game_id;

![Screenshot (36)](https://github.com/user-attachments/assets/0588fb04-4136-496b-b086-4fa40969a9e8)


