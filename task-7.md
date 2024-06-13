-- 1: film tablosunda bulunan filmleri rating de�erlerine g�re gruplay�n�z.
```
select rating, count(*) from film f 
group by rating;
```

-- 2: film tablosunda bulunan filmleri replacement_cost s�tununa g�re gruplad���m�zda film say�s� 50 den fazla olan replacement_cost de�erini ve kar��l�k gelen film say�s�n� s�ralay�n�z.
```
select replacement_cost, count(replacement_cost) from film f
group by replacement_cost
having count(replacement_cost) > 50
order by replacement_cost;
```

-- 3: customer tablosunda bulunan store_id de�erlerine kar��l�k gelen m��teri say�lar�n� nelerdir? 
```
select store_id, count(customer_id) from customer c
group by store_id ;
```

-- 4: city tablosunda bulunan �ehir verilerini country_id s�tununa g�re grupland�rd�ktan sonra en fazla �ehir say�s� bar�nd�ran country_id bilgisini ve �ehir say�s�n� payla��n�z.
```
select country_id, count(city) from city c
group by country_id
order by count(city) desc
limit 1;
```