# Week 3

### Assignment: Multiple Table Queries

### Question 1
select country.name as "country name", airport.name as "airport name"  from country, airport 
where airport.iso_country = country.iso_country and country.name = "Iceland";

![Screenshot (23)](https://github.com/user-attachments/assets/d92cdd67-dab7-4844-92dc-f8c4b04cb80a)

