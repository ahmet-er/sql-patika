-- �dev 11
---
--1: actor ve customer tablolar�nda bulunan first_name s�tunlar� i�in t�m verileri s�ralayal�m.
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
--2: actor ve customer tablolar�nda bulunan first_name s�tunlar� i�in kesi�en verileri s�ralayal�m.
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
--3: actor ve customer tablolar�nda bulunan first_name s�tunlar� i�in ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri s�ralayal�m.
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
--4: �lk 3 sorguyu tekrar eden veriler i�in de yapal�m.
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