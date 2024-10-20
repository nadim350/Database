# Week 3

### Assignment: Multiple Table Queries

### Question 1
select country.name as "country name", airport.name as "airport name"  from country, airport 
where airport.iso_country = country.iso_country and country.name = "Iceland";

![Screenshot (23)](https://github.com/user-attachments/assets/d92cdd67-dab7-4844-92dc-f8c4b04cb80a)

### Question 2
select airport.name as "Airport Name" from airport,country 
where airport.iso_country = country.iso_country and country.name = "France" and airport.type = "large_airport"; 

![Screenshot (24)](https://github.com/user-attachments/assets/096c86ee-69a4-44b9-b207-a1f4db42b6d9)

### Question 3
Select country.name as "country_name", airport.name as "airport_name" from airport,country 
where airport.iso_country = country.iso_country and country.continent = "AN";


![Screenshot (25)](https://github.com/user-attachments/assets/bc096e4e-5faf-45a4-a646-41e9bfac624c)


### Question 4
select elevation_ft from airport,game where game.location = ident and screen_name ="Heini";

![Screenshot (26)](https://github.com/user-attachments/assets/6260314d-955d-459f-bfd6-4cf0eca73ab4)

### Question 5
select elevation_ft * 0.3048 as "elevation_m" from airport,game where game.location = ident and screen_name ="Heini";

![Screenshot (27)](https://github.com/user-attachments/assets/22ca5527-01d4-486b-a20e-d016ea52f304)


### Question 6
select name from airport,game where location = ident and screen_name = "Ilkka";

![Screenshot (28)](https://github.com/user-attachments/assets/93b41389-4ec0-45df-bf31-b7be78d2cb89)


### Question 7
select country.name from airport,country,game 
where airport.iso_country = country.iso_country and location = ident and screen_name = "Ilkka";

![Screenshot (29)](https://github.com/user-attachments/assets/bf2a0391-6bb4-42f8-97ba-c33eb6e6b8a2)


### Question 8 
select name from goal, goal_reached, game  where game_id and goal.id = goal_id and screen_name = "Heini";


![Screenshot (30)](https://github.com/user-attachments/assets/681d3c2d-a226-4b7a-9d7b-88a8580d6cbd)


### Question 9
select airport.name from game, goal_reached, goal, airport 
where ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";

![Screenshot (31)](https://github.com/user-attachments/assets/d8c52d39-5a03-4c58-916a-cba321bf5952)


 ### Question 10
select country.name from game, goal_reached, goal, country, airport 
where airport.iso_country = country.iso_country and ident = location and game.id = game_id and goal.id = goal_id and screen_name = "Ilkka" and goal.name = "CLOUDS";

![Screenshot (32)](https://github.com/user-attachments/assets/37dc7042-a55e-41ca-838d-561710e67175)







