A�a��daki sorgu senaryolar�n� dvdrental �rnek veri taban� �zerinden ger�ekle�tiriniz.
---
-- 1: film tablosunda bulunan t�m s�tunlardaki verileri replacement cost de�eri 12.99 dan b�y�k e�it ve 16.99 k���k olma ko�uluyla s�ralay�n�z ( BETWEEN - AND yap�s�n� kullan�n�z.)

```
select * from film f 
where replacement_cost between 12.99 and 16.99;
```
---
-- 2: actor tablosunda bulunan first_name ve last_name s�tunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' de�erleri olmas� ko�uluyla s�ralay�n�z. ( IN operat�r�n� kullan�n�z.)
```
select first_name, last_name from actor
where first_name in ('Penelope', 'Nick', 'Ed');
```
---
-- 3: film tablosunda bulunan t�m s�tunlardaki verileri rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma ko�ullar�yla s�ralay�n�z. ( IN operat�r�n� kullan�n�z.)
```
select * from film f 
where rental_rate in (0.99, 2.99, 4.99) and replacement_cost in (12.99, 15.99, 28.99);
```