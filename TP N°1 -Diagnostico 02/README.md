# a) 
Crear la tabla marcas con los siguentes campos: "IdMarca, NombreMarca y NombreCiudad", ninguno de estos puede ser NULL y la PRIMARY KEY debe ser IdMarca que es un SMALLINT predeterminado en 1. Los otros campos son cadenas de caracteres.
``` 
CREATE TABLE MARCAS (
IdMarca SMALLINT NOT NULL DEFAULT 1,
NombreMarca CHAR(10) NOT NULL,
NombreCiudad CHAR(60) NOT NULL,
PRIMARY KEY (idMarca))
```
# b)
Crear la tabla coches, donde su PRIMARY KEY debe ser "codcoche" ademas debe tener los cambo nombre y modelo que son cadenas de caracteres.
```
CREATE TABLE COCHES (
codcoche SMALLINT NOT NULL,
nombre CHAR(15) NOT NULL,
modelo CHAR(10),
PRIMARY KEY (codcoche))
```
# c)
Crear la tabla marco declarando IdMarca y codcoche igual que en las tablas anteriores. La PRIMARY KEY se crea combinando IdMarca y codchoce. La tabla solo posee dos campos que hacen referencia al contenido de las otras tablas.
```
CREATE TABLE MARCO (
IdMarca SMALLINT NOT NULL,
codcoche SMALLINT NOT NULL,
PRIMARY KEY (cifm,codcoche),
FOREIGN KEY (cifm) REFERENCES MARCA,
FOREIGN KEY (codcoche) REFERENCES COCHE)
```
# d)
Insertar valores en la tabla marcas.
```
INSERT INTO MARCAS VALUES (1,'vw','Mar del Plata')
INSERT INTO MARCAS VALUES (2,'renault','Rosario')
INSERT INTO MARCAS VALUES (3,'fiat','Cordoba')
INSERT INTO MARCAS VALUES (4,'ford','Neuquen')
```
# e)
Mostrar toda la informacion en la tabla Marcas
```
SELECT * FROM MARCAS
```
# f)
Mostrar los valores almacenados en los campos NombreMarca y NombreCiudad.
```
SELECT nombre, ciudad FROM MARCAS
```
# g)
Mostrar los valores almacenados en los campos NombreMarca y NombreCiudad que correspondan al IdMarca con valor 2.
```
select nombre,ciudad from MARCAS where IdMarca = 2
```
# h)
Mostrar los valores almacaenados en los campos NombreMarca y NombreCiudad de la tabla marcas, donde NombreCiudad sea igual a 'Neuquen'.
```
select NombreMarca,ciudad from marca
where ciudad = 'Neuquen'
```
# i)
Mostrar los valores almacenados en los campos NombreMarca y NombreCiudad donde NombreCiudad comience con S
```
select nombre,ciudad
from marcas
where ciudad LIKE 'S%'
```
# j)
Realizar cambios en la tabla marcas cambiando el campo ciudad todos los campos que digan 'Jujuy' por 'Neuquen'
```
update marcas
set ciudad = 'Nuequen'
where ciudad = 'Jujuy'
```
