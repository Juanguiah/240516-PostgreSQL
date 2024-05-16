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
