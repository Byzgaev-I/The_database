# Домашнее задание к занятию «Базы данных» - `Бызгаев Александр`  
---
### Легенда  

Заказчик передал вам [файл в формате Excel](https://github.com/netology-code/sdb-homeworks/blob/main/12-01.md#:~:text=%D1%84%D0%B0%D0%B9%D0%BB%20%D0%B2%20%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%82%D0%B5%20Excel), в котором сформирован отчёт. 

На основе этого отчёта нужно выполнить следующие задания.

### Задание 1  
Опишите не менее семи таблиц, из которых состоит база данных:
- какие данные хранятся в этих таблицах;
- какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.
Приведите решение к следующему виду:

Сотрудники (
- идентификатор, первичный ключ, serial,
- фамилия varchar(50),
- ...
- идентификатор структурного подразделения, внешний ключ, integer).

### Решение  
