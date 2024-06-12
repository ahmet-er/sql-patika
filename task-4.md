Aþaðýdaki sorgu senaryolarýný dvdrental örnek veri tabaný üzerinden gerçekleþtiriniz.
---
-- 1: film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklý deðerleri sýralayýnýz.

```
select distinct replacement_cost from film;
```
---
-- 2: film tablosunda bulunan replacement_cost sütununda birbirinden farklý kaç tane veri vardýr?
```
select count(distinct replacement_cost) from film;
```
---
-- 3: film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile baþlar ve ayný zamanda rating 'G' ye eþittir?
```
select count(title) from film f 
where title like 'T%' and rating = 'G';
```
---

-- 4: country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluþmaktadýr?
```
select count(country) from country c 
where country like '_____';
```
---

-- 5: city tablosundaki þehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
```
select count(city) from city c 
where city like 'R%' or city like '%r';
```


