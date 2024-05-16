# 240516-PostgreSQL
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
