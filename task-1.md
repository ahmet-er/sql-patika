Aþaðýdaki sorgu senaryolarýný dvdrental örnek veri tabaný üzerinden gerçekleþtiriniz.
---
-- 1: film tablosunda bulunan title ve description sütunlarýndaki verileri sýralayýnýz.

```
select title, description from film;
```
---
-- 2: film tablosunda bulunan tüm sütunlardaki verileri film uzunluðu (length) 60 dan büyük VE 75 ten küçük olma koþullarýyla sýralayýnýz.
```select * from film
where length > 60 and length < 75;
```
---
-- 3: film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koþullarýyla sýralayýnýz.
```
select * from film
where rental_rate = 0.99 and (replacement_cost = 12.99 or replacement_cost = 28.99);
```
---

-- 4: customer tablosunda bulunan first_name sütunundaki deðeri 'Mary' olan müþterinin last_name sütunundaki deðeri nedir?
```
select last_name from customer 
where first_name = 'Mary';
```
---

-- 5: film tablosundaki uzunluðu(length) 50 ten büyük OLMAYIP ayný zamanda rental_rate deðeri 2.99 veya 4.99 OLMAYAN verileri sýralayýnýz.
```
select * from film 
where length < 50 and not (rental_rate = 2.99 or rental_rate = 4.99);
```