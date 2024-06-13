-- 1: test veritabanýnýzda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluþturalým.
```
create table employee (
	id int primary key,
	name varchar(50),
	birthday date,
	email varchar(100)
);
```

-- 2: Oluþturduðumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
```
insert into employee (id, name, birthday, email) values (1, 'Marion Coniam', '1961-01-24', 'mconiam0@blog.com');
insert into employee (id, name, birthday, email) values (2, 'Lazare Debill', '1945-10-24', 'ldebill1@woothemes.com');
insert into employee (id, name, birthday, email) values (3, 'Kiele Ogilvy', '1974-08-24', 'kogilvy2@scribd.com');
insert into employee (id, name, birthday, email) values (4, 'Daren Carmen', '1999-08-27', 'dcarmen3@last.fm');
insert into employee (id, name, birthday, email) values (5, 'Elroy Treverton', null, 'etreverton4@ovh.net');
insert into employee (id, name, birthday, email) values (6, 'Reina Luttger', '1946-10-07', 'rluttger5@un.org');
insert into employee (id, name, birthday, email) values (7, 'Pennie Toombs', '1900-06-29', 'ptoombs6@vkontakte.ru');
insert into employee (id, name, birthday, email) values (8, 'Mallory Kittredge', null, 'mkittredge7@networksolutions.com');
insert into employee (id, name, birthday, email) values (9, 'Nial Collinette', '1943-07-05', 'ncollinette8@boston.com');
insert into employee (id, name, birthday, email) values (10, 'Ingeberg Conroy', null, 'iconroy9@vimeo.com');
insert into employee (id, name, birthday, email) values (11, 'Orville Lewcock', '1930-08-14', 'olewcocka@arizona.edu');
insert into employee (id, name, birthday, email) values (12, 'Elinor Shovlin', '1975-12-19', 'eshovlinb@creativecommons.org');
insert into employee (id, name, birthday, email) values (13, 'Roobbie Fery', null, 'rferyc@hhs.gov');
insert into employee (id, name, birthday, email) values (14, 'Lila Tibbetts', '1950-08-28', 'ltibbettsd@nature.com');
insert into employee (id, name, birthday, email) values (15, 'Sol Baigrie', '1940-10-06', 'sbaigriee@altervista.org');
insert into employee (id, name, birthday, email) values (16, 'Justen De Luna', '1989-05-29', 'jdef@sitemeter.com');
insert into employee (id, name, birthday, email) values (17, 'Shamus Knottley', '1935-04-29', 'sknottleyg@themeforest.net');
insert into employee (id, name, birthday, email) values (18, 'Fulton Avard', '1982-04-03', 'favardh@marriott.com');
insert into employee (id, name, birthday, email) values (19, 'Nikola Thebe', '1977-06-17', 'nthebei@nature.com');
insert into employee (id, name, birthday, email) values (20, 'Valencia Wile', '1954-04-29', 'vwilej@weibo.com');
insert into employee (id, name, birthday, email) values (21, 'Tallulah Alkins', '1928-08-20', 'talkinsk@timesonline.co.uk');
insert into employee (id, name, birthday, email) values (22, 'Almeda Higford', '1932-03-01', 'ahigfordl@zdnet.com');
insert into employee (id, name, birthday, email) values (23, 'Jacquelynn Earland', '1923-07-01', 'jearlandm@bluehost.com');
insert into employee (id, name, birthday, email) values (24, 'Auria Giannassi', '1900-10-09', 'agiannassin@cornell.edu');
insert into employee (id, name, birthday, email) values (25, 'Almeria Dawidsohn', '1950-12-14', 'adawidsohno@uol.com.br');
insert into employee (id, name, birthday, email) values (26, 'Kimberlyn Mingardo', '1960-09-23', 'kmingardop@hubpages.com');
insert into employee (id, name, birthday, email) values (27, 'Beatrix Bowe', null, 'bboweq@mapy.cz');
insert into employee (id, name, birthday, email) values (28, 'Bjorn Rabier', '1999-01-12', 'brabierr@naver.com');
insert into employee (id, name, birthday, email) values (29, 'Selle Kezourec', '1919-02-15', 'skezourecs@rambler.ru');
insert into employee (id, name, birthday, email) values (30, 'Sabina Aris', '1917-03-08', 'sarist@indiatimes.com');
insert into employee (id, name, birthday, email) values (31, 'Meredith Rodenburgh', null, 'mrodenburghu@goo.ne.jp');
insert into employee (id, name, birthday, email) values (32, 'Ermina Willman', '1977-02-03', 'ewillmanv@spiegel.de');
insert into employee (id, name, birthday, email) values (33, 'Mark Blindmann', '1967-06-19', 'mblindmannw@unicef.org');
insert into employee (id, name, birthday, email) values (34, 'Pavel Trusler', '1947-01-08', 'ptruslerx@businessinsider.com');
insert into employee (id, name, birthday, email) values (35, 'Winni Doubleday', '1949-09-17', 'wdoubledayy@house.gov');
insert into employee (id, name, birthday, email) values (36, 'Veradis McLugish', '1991-11-18', 'vmclugishz@imageshack.us');
insert into employee (id, name, birthday, email) values (37, 'Laurella Lassen', '1911-05-01', 'llassen10@zimbio.com');
insert into employee (id, name, birthday, email) values (38, 'Purcell Harte', '1905-08-06', 'pharte11@npr.org');
insert into employee (id, name, birthday, email) values (39, 'Karon Humbie', '1957-08-13', 'khumbie12@umn.edu');
insert into employee (id, name, birthday, email) values (40, 'Ban Scriviner', '1979-01-25', 'bscriviner13@myspace.com');
insert into employee (id, name, birthday, email) values (41, 'Kipper Rewbottom', '1965-01-30', 'krewbottom14@exblog.jp');
insert into employee (id, name, birthday, email) values (42, 'Agathe Shearsby', '1960-07-28', 'ashearsby15@scientificamerican.com');
insert into employee (id, name, birthday, email) values (43, 'Klarika Ladley', '1980-03-25', 'kladley16@myspace.com');
insert into employee (id, name, birthday, email) values (44, 'Meggi Skyram', '1928-08-17', 'mskyram17@quantcast.com');
insert into employee (id, name, birthday, email) values (45, 'Carley Walling', '1903-11-24', 'cwalling18@artisteer.com');
insert into employee (id, name, birthday, email) values (46, 'Gardener Torricina', '1989-04-14', 'gtorricina19@boston.com');
insert into employee (id, name, birthday, email) values (47, 'Greer Dilrew', '1923-10-10', 'gdilrew1a@paypal.com');
insert into employee (id, name, birthday, email) values (48, 'Dell Molden', '1908-02-12', 'dmolden1b@time.com');
insert into employee (id, name, birthday, email) values (49, 'Baryram Chaudhry', '1933-05-01', 'bchaudhry1c@squarespace.com');
insert into employee (id, name, birthday, email) values (50, 'Felicle Allam', '1976-09-29', 'fallam1d@joomla.org');
```

-- 3: Sütunlarýn her birine göre diðer sütunlarý güncelleyecek 5 adet UPDATE iþlemi yapalým.
```
update employee 
set name = 'UPDATE'
where id between 10 and 15;
```


-- 4: Sütunlarýn her birine göre ilgili satýrý silecek 5 adet DELETE iþlemi yapalým.
```
delete from employee
where id between 25 and 30;
```