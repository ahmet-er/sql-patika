-- Ödev 11
---
--1: actor ve customer tablolarýnda bulunan first_name sütunlarý için tüm verileri sýralayalým.
```
(
select first_name from actor
)
union
(
select first_name from customer
);
```
---
--2: actor ve customer tablolarýnda bulunan first_name sütunlarý için kesiþen verileri sýralayalým.
```
(
select first_name from actor
)
intersect
(
select first_name from customer
);
```
----
--3: actor ve customer tablolarýnda bulunan first_name sütunlarý için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sýralayalým.
```
(
select first_name from actor
)
except
(
select first_name from customer
);
```
---
--4: Ýlk 3 sorguyu tekrar eden veriler için de yapalým.
```
(
select first_name from actor
)
union all
(
select first_name from customer
);
```
```
(
select first_name from actor
)
intersect all
(
select first_name from customer
);
```
```
(
select first_name from actor
)
except all
(
select first_name from customer
);
```