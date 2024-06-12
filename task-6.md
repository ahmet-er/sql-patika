-- 1: film tablosunda bulunan rental_rate s�tunundaki de�erlerin ortalamas� nedir?
```
select avg(rental_rate) from film;
```

-- 2: film tablosunda bulunan filmlerden ka� tanesi 'C' karakteri ile ba�lar?
```
select count(*) from film
where title like 'C%' ;
```

-- 3: film tablosunda bulunan filmlerden rental_rate de�eri 0.99 a e�it olan en uzun (length) film ka� dakikad�r?
```
select max(length) from film f 
where f.rental_rate in (0.99);
```

-- 4: film tablosunda bulunan filmlerin uzunlu�u 150 dakikadan b�y�k olanlar�na ait ka� farkl� replacement_cost de�eri vard�r?
```
select count(distinct replacement_cost) from film f 
where length > 150;
```
