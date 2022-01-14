# Lesson-3-SQL
CREATE TABLE products (
                          id SERIAL PRIMARY KEY,
                          productName VARCHAR(30) NOT NULL,
                          manufacturer VARCHAR(20) NOT NULL,
                          productCount INTEGER DEFAULT 0,
                          price NUMERIC
);
INSERT INTO products  (productName, manufacturer, productCount, price)
  VALUES ('iPhone X', 'Apple', 2, 71000),
         ('iPhone 8', 'Apple', 3, 56000),
         ('Galaxy S9', 'Samsung', 6, 56000),
         ('Galaxy S8 Plus', 'Samsung', 2, 46000),
         ('Desire 12', 'HTC', 3, 26000);
CREATE TABLE students (
                          id SERIAL PRIMARY KEY,
                          fist_name VARCHAR(30) NOT NULL,
                          last_name VARCHAR(20) NOT NULL,
                          data_birth_day DATE NOT NULL ,
                          email VARCHAR(50) NOT NULL
);
INSERT INTO students  (fist_name,last_name,data_birth_day,email)
  VALUES ('Nurmuhammed','Babaev','2000-05-18','nurmuhammed@gmail.com'),
         ('Elmirbek','Amanov','2005-04-14','elmirbek@gmail.com'),
         ('Kuttubek','Gaparov','2004-03-16','kuttbek@gmail.com'),
         ('Aktan','Albertov','2002-07-21','aktan@gmail.com');
CREATE TABLE cars (
                          id SERIAL PRIMARY KEY,
                          carName VARCHAR(30) NOT NULL,
                          made_in VARCHAR(20) NOT NULL,
                          data_birth_day DATE NOT NULL ,
                          price NUMERIC
);
INSERT INTO cars  (carName, made_in, data_birth_day, price)
VALUES ('Volvo','China','1990-01-01',100000),
       ('BMB','America','1991-02-02',150000),
       ('Mercedes','Germany','1999-03-03',200000),
       ('Audi','Turkey','1995-05-05',120000);

CREATE TABLE laptops (
                      id SERIAL PRIMARY KEY,
                      laptopName VARCHAR(30) NOT NULL,
                      made_in VARCHAR(20) NOT NULL,
                      data_birth_day DATE NOT NULL ,
                      price NUMERIC
);
INSERT INTO laptops  (laptopName, made_in, data_birth_day, price)
VALUES ('Windows','China','1990-01-01',50000),
       ('Macos','America','1991-02-02',75000),
       ('Lenovo','Germany','1999-03-03',20000);
CREATE TABLE fruits (
                          id SERIAL PRIMARY KEY,
                          fruitName VARCHAR(30) NOT NULL,
                          styl VARCHAR(20) NOT NULL,
                          productCount INTEGER NOT NULL ,
                          price NUMERIC
);
INSERT INTO fruits(fruitName, styl,productCount, price)
VALUES ('Alma','svejyi',20,60),
       ('Banan','staryi',10,50),
       ('Alcha','svejyi',12,100);
CREATE TABLE chairs (
                          id SERIAL PRIMARY KEY,
                          toWight INT NOT NULL,
                          bigOrMoll VARCHAR(20) NOT NULL,
                          made_in VARCHAR(20) NOT NULL,
                          price NUMERIC
);
INSERT INTO chairs(toWight, bigOrMoll, made_in, price)
VALUES (4,'Moll','China',1200),
       (10,'Big','China',8000),
       (5,'Moll','America',1500),
       (11,'Big','America',9000);
CREATE TABLE golds (
                      id SERIAL PRIMARY KEY,
                      toWight INT NOT NULL,
                      made_in VARCHAR(20) NOT NULL,
                      price NUMERIC
);
INSERT INTO golds(toWight, made_in, price)
VALUES (1,'America',24809),
       (1,'Russian',1850000),
       (1,'Kyrgyzstan',2103820);
CREATE TABLE teapot (
                         id SERIAL PRIMARY KEY,
                         waiterName VARCHAR(30) NOT NULL,
                         how_many_people INT NOT NULL,
                         data_birth_day DATE NOT NULL ,
                         foodName VARCHAR(30)NOT NULL ,
                         priceOfTheFood NUMERIC
);
INSERT INTO teapot(waiterName, how_many_people, data_birth_day,foodName, priceOfTheFood)
 VALUES ('Nurtilek',10,'2000-05-08','Lapsha',200),
        ('Nurmuhammed',9,'2000-05-18','Manty',150),
        ('Kuttubek',14,'2004-03-28','Shorpo',120);

CREATE TABLE teacher (
                        id SERIAL PRIMARY KEY,
                       fistName VARCHAR(30) NOT NULL,
                        lastName VARCHAR(30) NOT NULL,
                        data_birth_day DATE NOT NULL ,
                        lesson VARCHAR(30)NOT NULL ,
                        zarplata NUMERIC
);
INSERT INTO teacher(fistName, lastName, data_birth_day, lesson, zarplata)
 VALUES ('Kuti','Gaparov','1998-01-01','Matematika',20000),
        ('Muhammed','Allanov','1999-09-11','Java',40000),
        ('Aktan','Majitov','2002-07-01','English',100000);

CREATE TABLE volonter (
                         id SERIAL PRIMARY KEY,
                         fistName VARCHAR(30) NOT NULL,
                         lastName VARCHAR(30) NOT NULL,
                         data_birth_day DATE NOT NULL ,
                         zarplata  VARCHAR(30)NOT NULL

);
INSERT INTO volonter(fistName, lastName, data_birth_day, zarplata)
VALUES ('Nurik','Bbabev','2000-05-18','Besplatno'),
       ('Kuttubek','Gaparov','2004-05-01','Besplatno'),
       ('Elmirbek','Mapaev','2005-03-28','Besplatno');

DROP TABLE laptops;


