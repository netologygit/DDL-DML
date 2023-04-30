SQL Часть 1 - Игуменова Екатерина


Упражнение 1

SELECT distinct district  FROM sakila.address where district LIKE 'K%a' and district not like '% %' ;

![ex 1](https://user-images.githubusercontent.com/123411071/235345442-b9418773-2b97-4938-8e09-6c2b4fd791f0.png)



Упражнение 2

select * from payment p where payment_date between "2005-06-15" and "2005-06-18 23:59:59" and amount > 10.00;

![ex 2](https://user-images.githubusercontent.com/123411071/235345435-4d102611-4d24-4ac3-8f64-a8135c5704df.png)



Упражнение 3

select * from rental r order by rental_date desc LIMIT 5;

![ex 3](https://user-images.githubusercontent.com/123411071/235345438-f78f0ab2-a29d-4126-b440-f0d915da4f02.png)



Упражнение 4

select replace(lower(first_name),'ll', 'pp'), lower(last_name) from customer c where first_name in ( "Kelly" , "Willie" ) and active = 1;

![ex 4](https://user-images.githubusercontent.com/123411071/235345440-de1b559a-fa91-4f08-b6b6-0458eecbf559.png)



