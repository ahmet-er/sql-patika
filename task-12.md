-- Ödev 12
---
-- 1: film tablosunda film uzunluðu length sütununda gösterilmektedir. Uzunluðu ortalama film uzunluðundan fazla kaç tane film vardýr?
```
 select count(*) 
 from film
 where length > 
 (
 	select avg(length) from film
 );
```
---
-- 2: film tablosunda en yüksek rental_rate deðerine sahip kaç tane film vardýr?
```
select count(*)
from film
where rental_rate =
(
	select max(rental_rate) 
	from film 
);
```
---
-- 3: film tablosunda en düþük rental_rate ve en düþük replacement_cost deðerlerine sahip filmleri sýralayýnýz.
```
select * 
from film
where rental_rate = (select min(rental_rate) from film)
and replacement_cost = (select min(replacement_cost) from film)
order by rental_rate, replacement_cost;
```
---
-- 4: payment tablosunda en fazla sayýda alýþveriþ yapan müþterileri(customer) sýralayýnýz.
```
select *
from customer
where customer_id in
(
	select customer_id 
	from payment
	group by customer_id 
	having count(*) = 
	(
		select max(payment_count)
		from
		(
			select count(*) as payment_count
			from payment
			group by customer_id 
		) as counts
	) 
)
order by customer_id;
```