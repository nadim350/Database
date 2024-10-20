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

![screenshot](/Screenshots/SingleTable_4.png)

### Question 5
select name from country where name like "F%";
![screenshot](/Screenshots/SingleTable_5.png)

### Question 6
select name from country where name like "%F%";
![screenshot](/Screenshots/SingleTable_6.png)

### Question 7
select location from game where screen_name = "Vesa";
![screenshot](/Screenshots/SingleTable_7.png)

### Question 8
select co2_consumed from game where screen_name = "Ilkka";
![screenshot](/Screenshots/SingleTable_8.png)

### Question 9
select distinct co2_budget from game;
![screenshot](/Screenshots/SingleTable_9.png)

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
![screenshot](/Screenshots/SingleTable_10.png)
