�dev 9
---
--1: city tablosu ile country tablosunda bulunan �ehir (city) ve �lke (country) isimlerini birlikte g�rebilece�imiz INNER JOIN sorgusunu yaz�n�z.
```
select country.country, city.city from country
inner join city on country.country_id = city.country_id;
```
---
--2: customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte g�rebilece�imiz INNER JOIN sorgusunu yaz�n�z.
```
select payment.payment_id, customer.first_name, customer.last_name from customer
inner join payment on customer.customer_id = payment.customer_id;
```
---
--3: customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte g�rebilece�imiz INNER JOIN sorgusunu yaz�n�z.
```
select rental.rental_id, customer.first_name, customer.last_name from customer
inner join rental on customer.customer_id = rental.customer_id;
```
