-- �dev 12
---
-- 1: film tablosunda film uzunlu�u length s�tununda g�sterilmektedir. Uzunlu�u ortalama film uzunlu�undan fazla ka� tane film vard�r?
```
 select count(*) 
 from film
 where length > 
 (
 	select avg(length) from film
 );
```
---
-- 2: film tablosunda en y�ksek rental_rate de�erine sahip ka� tane film vard�r?
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
-- 3: film tablosunda en d���k rental_rate ve en d���k replacement_cost de�erlerine sahip filmleri s�ralay�n�z.
```
select * 
from film
where rental_rate = (select min(rental_rate) from film)
and replacement_cost = (select min(replacement_cost) from film)
order by rental_rate, replacement_cost;
```
---
-- 4: payment tablosunda en fazla say�da al��veri� yapan m��terileri(customer) s�ralay�n�z.
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