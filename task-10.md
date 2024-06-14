-- Ödev 10
---
--1: city tablosu ile country tablosunda bulunan þehir (city) ve ülke (country) isimlerini birlikte görebileceðimiz LEFT JOIN sorgusunu yazýnýz.
```
select city, country from country
left join city on city.country_id = country.country_id; 
```
---
--2: customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceðimiz RIGHT JOIN sorgusunu yazýnýz.
```
select payment.payment_id, customer.first_name, customer.last_name from customer
right join payment on payment.customer_id = customer.customer_id;
```
---
--3: customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceðimiz FULL JOIN sorgusunu yazýnýz.
```
select rental.rental_id, customer.first_name, customer.last_name from customer
full outer join rental on customer.customer_id = rental.customer_id;
```