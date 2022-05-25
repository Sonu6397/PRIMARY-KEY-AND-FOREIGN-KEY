# PRIMARY-KEY-AND-FOREIGN-KEY

====================================================PRIMARY KEY TABLE T1=================================================================
create table T1(Id int primary key identity, Name varchar(50),Email varchar(50),Address varchar(50), Salary money,Gender varchar(50))
insert into T1 values
('sonu','sonu@gmail.com','rampur',25000,'male'),
('vimal','vimal@gmail.com','bijnor',15000,'male'),
('neha','neha@gmail.com','amwala',23000,'female'),
('khusi','khusi@gmail.com','moradabad',27000,'female'),
('deep','deep@gmail.com','bareilly',21000,'male')
select * from t1
select * from t2
============================================================FOREIGN KEY OF TABLE T2==========================================================
insert into T2 values
('sonu','sonu@gmail.com','rampur',25000,'male',2),
('vimal','vimal@gmail.com','bijnor',15000,'male',1),
('neha','neha@gmail.com','amwala',23000,'female',2),
('khusi','khusi@gmail.com','moradabad',27000,'female',4),
('deep','deep@gmail.com','bareilly',21000,'male',3)
create table  T2(Id int primary key identity,Name varchar(50), Email varchar(50), Address varchar(50),salary money, Gender varchar(50),  dpt_ID int  foreign key references t1 (Id) )
