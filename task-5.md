Aþaðýdaki sorgu senaryolarýný dvdrental örnek veri tabaný üzerinden gerçekleþtiriniz.
---
-- 1: film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sýralayýnýz.

```
select title from film
where title like '%n'
limit 5;
```
---
-- 2: film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kýsa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sýralayýnýz.
```
select title from film f 
where title like '%n'
limit 5
offset 5;
```
---
-- 3: customer tablosunda bulunan last_name sütununa göre azalan yapýlan sýralamada store_id 1 olmak koþuluyla ilk 4 veriyi sýralayýnýz.
```
select * from customer c 
where store_id = 1
order by last_name desc 
limit 4;
```