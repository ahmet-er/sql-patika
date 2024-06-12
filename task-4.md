A�a��daki sorgu senaryolar�n� dvdrental �rnek veri taban� �zerinden ger�ekle�tiriniz.
---
-- 1: film tablosunda bulunan replacement_cost s�tununda bulunan birbirinden farkl� de�erleri s�ralay�n�z.

```
select distinct replacement_cost from film;
```
---
-- 2: film tablosunda bulunan replacement_cost s�tununda birbirinden farkl� ka� tane veri vard�r?
```
select count(distinct replacement_cost) from film;
```
---
-- 3: film tablosunda bulunan film isimlerinde (title) ka� tanesini T karakteri ile ba�lar ve ayn� zamanda rating 'G' ye e�ittir?
```
select count(title) from film f 
where title like 'T%' and rating = 'G';
```
---

-- 4: country tablosunda bulunan �lke isimlerinden (country) ka� tanesi 5 karakterden olu�maktad�r?
```
select count(country) from country c 
where country like '_____';
```
---

-- 5: city tablosundaki �ehir isimlerinin ka� tanesi 'R' veya r karakteri ile biter?
```
select count(city) from city c 
where city like 'R%' or city like '%r';
```


