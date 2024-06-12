-- 1: film tablosunda bulunan rental_rate sütunundaki deðerlerin ortalamasý nedir?
```
select avg(rental_rate) from film;
```

-- 2: film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile baþlar?
```
select count(*) from film
where title like 'C%' ;
```

-- 3: film tablosunda bulunan filmlerden rental_rate deðeri 0.99 a eþit olan en uzun (length) film kaç dakikadýr?
```
select max(length) from film f 
where f.rental_rate in (0.99);
```

-- 4: film tablosunda bulunan filmlerin uzunluðu 150 dakikadan büyük olanlarýna ait kaç farklý replacement_cost deðeri vardýr?
```
select count(distinct replacement_cost) from film f 
where length > 150;
```
