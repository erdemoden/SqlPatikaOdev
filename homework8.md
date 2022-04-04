1.Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
````SQL
 CREATE TABLE employee (
 	id SERIAL,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
 )
````
2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
````SQL
insert into employee (name, birthday, email) values ('Wesley', '1998-10-12', 'wajsik0@unblog.fr');
insert into employee (name, birthday, email) values ('Malcolm', '1998-11-17', 'mwoodger1@nba.com');
insert into employee (name, birthday, email) values ('Laraine', '1996-09-07', 'landreasson2@cafepress.com');
insert into employee (name, birthday, email) values ('Emilia', '2001-07-12', 'esant3@ustream.tv');
insert into employee (name, birthday, email) values ('Teador', '2000-10-18', 'tquartermain4@chron.com');
````
3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
````SQL
UPDATE employee SET name = 'Emirhan', birthday = '2001-03-22',email = 'dev.emirhanay@gmail.com' WHERE id = 2;
````
4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
````SQL
DELETE FROM employee WHERE id = 2;
````
