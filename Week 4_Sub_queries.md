# Week 4

### Assignment: Subqueries

### Question 1
select name from country where iso_country in (select iso_country from airport where name like "Satsuma%");

![Screenshot (37)](https://github.com/user-attachments/assets/4c5243e9-86fd-4769-b1bd-0ed7012f15cf)


### Question 2
select name from airport where iso_country in (select iso_country from country where country.name = "Monaco");

![Screenshot (38)](https://github.com/user-attachments/assets/a6fbaacd-a76c-4736-b60d-0d10affdf99b)


### Question 3
Select screen_name from game where id in(select game_id 
from goal_reached where goal_id in(select id  from goal where name ="CLOUDS"));

![Screenshot (39)](https://github.com/user-attachments/assets/ef634097-b81f-475e-bb3f-5eee1051d85a)


### Question 4
Select country.name from country where iso_country not in (select airport.iso_country from airport);


![Screenshot (40)](https://github.com/user-attachments/assets/417d8d4d-a14a-44e2-b4b2-87dddf826603)



### Question 5
select name from goal where id not in (select goal.id from goal, goal_reached, game where game.id = game_id and goal.id = goal_id and screen_name = "Heini");

![Screenshot (41)](https://github.com/user-attachments/assets/f38de1dc-f79f-488a-bf6a-8d53ff4d6d86)


