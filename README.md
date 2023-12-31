# Домашнее задание к занятию «Базы данных» - `Бызгаев Александр`  
---
### Легенда  

Заказчик передал вам [файл в формате Excel](https://github.com/netology-code/sdb-homeworks/blob/main/resources/hw-12-1.xlsx), в котором сформирован отчёт. 

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

Сотрудник(
  - Идентификатор, первичный ключ, порядковый номер сотрудника, serial
  - Фамилия, varchar(50)
  - Имя, varchar(50)
  - Отчество, varchar(50)
  - должность id , integer
  - дата найма (date)
  - id_проекта, внешний ключ, integer
  - id подразделения, внешний ключ, integer
  - оклад, numeric  
)

Должность(
  - должность id, первичный ключ, integer
  - должность, varchar(50)
  - id подразделения, внешний ключ, integer
  - оклад, integer   
)

Тип подразделения( 
  - id тип подразделения, первичный ключ, integer
  - тип подразделения, varchar(50)  
)

Структурное подразделение(
  - id тип подразделения, первичный ключ, integer
  - тип подразделения, varchar(50)
  - адрес id, внешний ключ integer
  - id тип подразделения, внешний ключ, integer   
)

Адрес_филиала (
  - адрес id, первичный ключ, integer
  - адрес varchar(50)
  - город id, integer   
)

Регион (
  - регион_id, первичный ключ, integer
  - название региона, varchar(50)  
)

Город (
  - Город_id, первичный ключ, integer
  - Название города - varchar (50)    
)

Проект на который назначен (
  - id_проекта, первичный ключ, integer
  - проект на который назначен varchar(100)   
)
---
