# 240516-PostgreSQL
Despues de abrir DBeaver y crearo una base de datos y un tabla en PostgreSQL, con estos comandos DML (Data Manipulation Language), se insertan, actualizan y se borran datos en la base de datos, y con el comando DQL(Data Query Language) select se consultan datos de la siguiente manera:

```insert into public.vehiculos (marca, modelo, linea, placa, color) 
values ('Ford', '2012', 'Fiesta', 'KKK262', 'Plata'),
('Marza', '2012', '2', 'EPU504', 'Gris')

SELECT id, marca, modelo, linea, placa, color
FROM public.vehiculos;

SELECT * FROM public.vehiculos;

update public.vehiculos 
set modelo = '2022'
where id =1

delete from public.vehiculos 
where id =2```

Ahora creemos una base de datos y tabla con los comandos DDL (Data Definition Language) y luego eliminimemos columnas, alteremosla, agreguemosla de nuevo, y eliminemos los datos con el siguiente script:

```create database "Compra-venta"

create table cliente(
id serial primary key,
nombres varchar(50) not null,
apellidos  varchar(50) not null,
telefono  varchar(10) not null,
activo boolean,
direccion  varchar(100) not null
)

drop database "DB_name"
drop table "Esquema.Tabla_name"

alter table cliente add email varchar(50) not null

alter table cliente drop activo

alter table cliente add activo boolean

alter table cliente alter column activo type varchar(20)

alter table cliente drop activo

alter table cliente add activo boolean

insert into public.cliente (nombres, apellidos, telefono, direccion, email, activo)
values ('Juan', 'Arcila', '3003007000', 'Cra 42a 30', 'juarcila@gmail.com', true),
('Andrea', 'Ochoa', '3003009000', 'Amarello In', 'andrea8amo@hotmail.com', true)

select * from public.cliente 
truncate public.cliente ```
