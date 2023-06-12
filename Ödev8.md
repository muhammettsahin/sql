1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```javascript
CREATE TABLE employee(
	id SERIAL PRIMARY KEY,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);
	
```
2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

```javascript
insert into employee (name, birthday, email) values ('Lilli', '1981-11-21', 'lsendall0@jalbum.net');
insert into employee (name, birthday, email) values ('Beauregard', '1994-05-31', 'bmetheringham1@imgur.com');
insert into employee (name, birthday, email) values ('Colver', '1999-06-10', 'cgrzesiak2@symantec.com');
insert into employee (name, birthday, email) values ('Faustina', '1986-01-14', 'fpochon3@cdc.gov');
insert into employee (name, birthday, email) values ('Alecia', '1998-08-22', 'agoldby4@wp.com');
insert into employee (name, birthday, email) values ('Sterling', '1996-07-16', 'sowthwaite5@homestead.com');
insert into employee (name, birthday, email) values ('Regen', '2002-06-20', 'rlally6@unblog.fr');
insert into employee (name, birthday, email) values ('Ingamar', '1989-04-27', 'icoleshill7@ning.com');
insert into employee (name, birthday, email) values ('Rutter', '1989-01-27', 'rscholar8@nhs.uk');
insert into employee (name, birthday, email) values ('Ephrem', '1998-01-27', 'ejedrysik9@pcworld.com');
insert into employee (name, birthday, email) values ('Rasla', '1982-12-22', 'rwakeforda@exblog.jp');
insert into employee (name, birthday, email) values ('Cristin', null, 'cdyersonb@163.com');
insert into employee (name, birthday, email) values ('Elladine', '1981-01-22', 'echangc@4shared.com');
insert into employee (name, birthday, email) values ('Emmett', '1987-07-17', 'elearyd@studiopress.com');
insert into employee (name, birthday, email) values ('Gage', '1981-02-10', 'gbairnsfathere@reuters.com');
insert into employee (name, birthday, email) values ('Graehme', '1993-10-03', 'gwillsf@nba.com');
insert into employee (name, birthday, email) values ('Jena', '1991-01-01', 'jvarvarag@twitter.com');
insert into employee (name, birthday, email) values ('Witty', '1996-04-23', 'wdilstonh@goo.ne.jp');
insert into employee (name, birthday, email) values ('Torr', '1982-01-23', 'tjeani@state.gov');
insert into employee (name, birthday, email) values ('Phillip', '1998-05-06', 'pbrownriggj@marketwatch.com');
insert into employee (name, birthday, email) values ('Mac', '1985-08-06', 'mwisniowskik@fda.gov');
insert into employee (name, birthday, email) values ('Patsy', '1989-07-30', 'pgoingl@tamu.edu');
insert into employee (name, birthday, email) values ('Noni', '1989-11-20', 'npankettmanm@mlb.com');
insert into employee (name, birthday, email) values ('Abrahan', '1998-04-12', 'awoofn@latimes.com');
insert into employee (name, birthday, email) values ('Tiff', '2001-01-18', 'tramsbyo@buzzfeed.com');
insert into employee (name, birthday, email) values ('Glen', '2000-06-18', 'gbottrellp@cisco.com');
insert into employee (name, birthday, email) values ('Reinaldos', '1981-05-12', 'rpetrikq@a8.net');
insert into employee (name, birthday, email) values ('Gloriana', '1992-03-16', 'gstobber@google.cn');
insert into employee (name, birthday, email) values ('Trina', '1992-10-24', 'tfritschels@yellowpages.com');
insert into employee (name, birthday, email) values ('Hercule', '1998-01-10', 'hloguet@pen.io');
insert into employee (name, birthday, email) values ('Carole', '1991-04-28', 'craffonu@fda.gov');
insert into employee (name, birthday, email) values ('Anabel', '1983-03-25', 'ayegoshinv@sphinn.com');
insert into employee (name, birthday, email) values ('Karol', '1995-11-15', 'kmedendorpw@mail.ru');
insert into employee (name, birthday, email) values ('Lou', '1986-04-12', 'ldentonx@pbs.org');
insert into employee (name, birthday, email) values ('Ruthy', '1999-09-02', 'rcancellarioy@accuweather.com');
insert into employee (name, birthday, email) values ('Curran', '1999-08-09', 'cbrundellz@foxnews.com');
insert into employee (name, birthday, email) values ('Matthus', '1993-10-24', 'mhiggoe10@cisco.com');
insert into employee (name, birthday, email) values ('Roselia', '1997-06-13', 'rmcinility11@yelp.com');
insert into employee (name, birthday, email) values ('Job', null, 'jlarkin12@whitehouse.gov');
insert into employee (name, birthday, email) values ('Stephanus', '1993-07-26', 'skirke13@aboutads.info');
insert into employee (name, birthday, email) values ('Obadiah', '1981-04-11', 'owinspeare14@people.com.cn');
insert into employee (name, birthday, email) values ('Marget', null, 'mblazi15@networkadvertising.org');
insert into employee (name, birthday, email) values ('Babs', '2002-12-04', 'bgonsalvez16@house.gov');
insert into employee (name, birthday, email) values ('Lorna', null, 'lameerbeg17@123-reg.co.uk');
insert into employee (name, birthday, email) values ('Darnall', '1995-10-05', 'dscarsbrook18@bandcamp.com');
insert into employee (name, birthday, email) values ('Padgett', '1987-12-28', 'pbradnock19@liveinternet.ru');
insert into employee (name, birthday, email) values ('Sanderson', '1986-02-23', 'scossam1a@usa.gov');
insert into employee (name, birthday, email) values ('Rodi', null, 'rbeels1b@homestead.com');
insert into employee (name, birthday, email) values ('Lorelei', '1989-10-29', 'lpriest1c@loc.gov');
insert into employee (name, birthday, email) values ('Jose', '2001-02-06', 'jkesteven1d@shutterfly.com');
	
```

3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```javascript
UPDATE employee
SET name = 'Ryan'
WHERE id = 3;

UPDATE employee
SET birthday = '1993-04-29'
WHERE name = 'Lilli';

UPDATE employee
SET email = 'besiktas@besiktas.com'
WHERE id = 35;

UPDATE employee
SET email = 'besiktas@besiktas.com'
WHERE email = 'skirke13@aboutads.info';

UPDATE employee
SET name = 'Jack'
WHERE name = 'Job';
	
```
4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```javascript
DELETE FROM employee
WHERE name = 'Faustina';

DELETE FROM employee
WHERE birthday = '1993-04-29';

DELETE FROM employee
WHERE id = 39;

DELETE FROM employee
WHERE email = 'agoldby4@wp.com';

DELETE FROM employee
WHERE name LIKE 'R%';
	
```
