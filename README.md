# PR
### SQL-request 

**ШИФТ интенсив**

1) Выберете все услуги для членов клуба
```
SELECT *
FROM cd.facilities;
```
2) Выберете только наименование услуги и обе стоимости
```
SELECT name, membercost, guestcost
FROM cd.facilities;
```
3) Выберете услуги, которые содержат слово 'Tennis'
```
SELECT name
FROM cd.facilities
WHERE name LIKE '%Tennis%';
```
4) Выберите 10 упорядоченных фамилий членов клуба без дубликатов
```
SELECT DISTINCT surname
FROM cd.members
ORDER BY surname ASC
LIMIT 10;
```
5) Добавьте новую услугу
```
INSERT INTO cd.facilities
	(facid, name, membercost, guestcost, initialoutlay)
VALUES
	(9, 'Spa', 20, 30, 100000, 800);
```
6) Обновите стоимость услуги из п.5 для гостей на 50
```
UPDATE cd.facilities
SET guestcost = '50'
WHERE name = 'Spa';
```
7) Удалите добавленную в п.5 услугу
```
DELETE
FROM cd.facilities
WHERE facid = 9;
```
8) Выведите количество услуг
```
SELECT COUNT(facid) AS 'Количество услуг'
FROM cd.facilities;
```
**Stepik курс**

1. Создание таблицы Auto
   
![image](https://github.com/user-attachments/assets/a3682f0a-3839-4c7d-b761-8468d77381b6)

2. Заполнить таблицу Auto 10 записями (10 авто)

![image](https://github.com/user-attachments/assets/ddc6bf1d-e428-4bf9-b368-10292b2976ef)

3. Создать запрос по выдаче авто только марки Toyota

![image](https://github.com/user-attachments/assets/b5cdc75c-2e47-4785-840b-86e02511d65e)

4. Создать запрос по выдаче последних 3 авто

![image](https://github.com/user-attachments/assets/c386be60-dd20-4e3b-87d8-12bd37b37755)

5. Создать запрос по выдаче самого дорого авто

![image](https://github.com/user-attachments/assets/088eb0e6-d7b0-4cb8-897f-d4bd799349ee)

6. Создать запрос по выдаче авто стоимостью 1 000 000 рублей и более

![image](https://github.com/user-attachments/assets/9542fb0e-d2cc-4c67-9f46-b29c01d07813)
