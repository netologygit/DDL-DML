
SQL. Часть 2 - Игуменова Екатерина

***Упражнение 1***

```sql

select concat(s2.first_name,' ', s2.last_name) as "имя фамилия"  ,c2.city as "город" , count(*) as "кол-во пользователей"

from customer c 

inner join store s on c.store_id = s.store_id

join address a on s.address_id = a.address_id 

join city c2 on a.city_id = c2.city_id

join staff s2 on s.manager_staff_id = s2.staff_id 

group by c.store_id having count(c.store_id) > 300;

```

![ex 1](https://user-images.githubusercontent.com/123411071/235351104-a35d9f6a-05bd-4f2d-9fe5-db173e215558.png)


***Упражнение 2***

```sql

select count(*) from film f2 where `length` > (select avg(length) 
from film f);

```


![ex 2](https://user-images.githubusercontent.com/123411071/235351108-cc165d2b-c916-40dd-ba94-a24a47d79466.png)


***Упражнение 3***

```sql


select month(p.payment_date) as "месяц", sum(p.amount) as "сумма платежей", count(p.rental_id) as "кол-во аренд" 

from payment p

group by month(p.payment_date)

order by sum(p.amount) desc limit 1;

```

![ex 3](https://user-images.githubusercontent.com/123411071/235351115-2eb5c46b-e8fd-41e3-8902-0f247555c542.png)
