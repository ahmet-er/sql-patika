A�a��daki sorgu senaryolar�n� dvdrental �rnek veri taban� �zerinden ger�ekle�tiriniz.
---
-- 1: film tablosunda bulunan title ve description s�tunlar�ndaki verileri s�ralay�n�z.

```
select title, description from film;
```
---
-- 2: film tablosunda bulunan t�m s�tunlardaki verileri film uzunlu�u (length) 60 dan b�y�k VE 75 ten k���k olma ko�ullar�yla s�ralay�n�z.
```
select * from film
where length > 60 and length < 75;
```
---
-- 3: film tablosunda bulunan t�m s�tunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma ko�ullar�yla s�ralay�n�z.
```
select * from film
where rental_rate = 0.99 and (replacement_cost = 12.99 or replacement_cost = 28.99);
```
---

-- 4: customer tablosunda bulunan first_name s�tunundaki de�eri 'Mary' olan m��terinin last_name s�tunundaki de�eri nedir?
```
select last_name from customer 
where first_name = 'Mary';
```
---

-- 5: film tablosundaki uzunlu�u(length) 50 ten b�y�k OLMAYIP ayn� zamanda rental_rate de�eri 2.99 veya 4.99 OLMAYAN verileri s�ralay�n�z.
```
select * from film 
where length < 50 and not (rental_rate = 2.99 or rental_rate = 4.99);
```