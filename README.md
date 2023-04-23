# Домашнее задание к занятию "`Название занятия`" - `Фамилия и имя студента`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1
![create_user](https://user-images.githubusercontent.com/123411071/233840415-23a181b5-88e3-4d60-87bc-b55529eb697a.png)
![grant](https://user-images.githubusercontent.com/123411071/233840420-739aeb57-6db9-4dcd-8cae-c69a87859a24.png)
![select user](https://user-images.githubusercontent.com/123411071/233840426-62790672-adc2-4b4f-a761-a721baac8c79.png)
![show grant](https://user-images.githubusercontent.com/123411071/233840439-be96eb9c-c134-4434-bd91-0db2a847839b.png)
![alter user](https://user-images.githubusercontent.com/123411071/233840453-16b2e86e-9365-44fa-a9ef-d7fba1fac251.png)
![ER diagramma](https://user-images.githubusercontent.com/123411071/233840464-c051aa0c-cb0e-4f34-be37-fc4baed0fb8c.png)
![dump db](https://user-images.githubusercontent.com/123411071/233840476-0535bada-2baa-47d2-a5fb-8b1e1f648755.png)

1.2 CREATE USER 'sys_temp' IDENTIFIED BY 'Pass1234567';

1.3 SELECT user FROM mysql.user;

1.4 GRANT ALL PRIVILEGES ON *.* TO 'sys_temp';

1.5 show grants for 'sys_temp';

1.6 ALTER USER 'sys_temp' IDENTIFIED WITH mysql_native_password BY 'Pass1234567';

###Задание 2

Название таблицы | Название первичного ключа
         
actor    -                       actor_id  
address    -                     address_id  
category    -                    category_id  
city   -                         city_id   
country    -                     country_id  
customer   -                     customer_id  
film    -                        film_id  
film_actor  -                    actor_id, film_id  
film_category -                  film_id, category_id  
film_text   -                    film_id  
inventory  -                     inventory_id  
language  -                      language_id  
payment  -                       payment_id  
rental   -                       rental_id  
staff  -                         staff_id
store   -                        store_id, manager_staff_id

![zadaniye_2](https://user-images.githubusercontent.com/123411071/233840496-ea2060cf-9d39-480b-a302-b15e316de3f3.png)
