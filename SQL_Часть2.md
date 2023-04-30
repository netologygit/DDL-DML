
SQL. Часть 2 - Игуменова Екатерина

Упражнение 1

select concat(s2.first_name,' ', s2.last_name) as "имя фамилия"  ,c2.city as "город" , count(*) as "кол-во пользователей"
from customer c 
inner join store s on c.store_id = s.store_id
join address a on s.address_id = a.address_id 
join city c2 on a.city_id = c2.city_id
join staff s2 on s.manager_staff_id = s2.staff_id 
group by c.store_id having count(c.store_id) > 300;




Упражнение 2

select count(*) from film f2 where `length` > (select avg(length) 
from film f);



Упражнение 3

select month(p.payment_date) as "месяц", sum(p.amount) as "сумма платежей", count(p.rental_id) as "кол-во аренд" 
from payment p
group by month(p.payment_date)
order by sum(p.amount) desc limit 1;


