-- 1: film tablosunda bulunan filmleri rating deðerlerine göre gruplayýnýz.
```
select rating, count(*) from film f 
group by rating;
```

-- 2: film tablosunda bulunan filmleri replacement_cost sütununa göre grupladýðýmýzda film sayýsý 50 den fazla olan replacement_cost deðerini ve karþýlýk gelen film sayýsýný sýralayýnýz.
```
select replacement_cost, count(replacement_cost) from film f
group by replacement_cost
having count(replacement_cost) > 50
order by replacement_cost;
```

-- 3: customer tablosunda bulunan store_id deðerlerine karþýlýk gelen müþteri sayýlarýný nelerdir? 
```
select store_id, count(customer_id) from customer c
group by store_id ;
```

-- 4: city tablosunda bulunan þehir verilerini country_id sütununa göre gruplandýrdýktan sonra en fazla þehir sayýsý barýndýran country_id bilgisini ve þehir sayýsýný paylaþýnýz.
```
select country_id, count(city) from city c
group by country_id
order by count(city) desc
limit 1;
```