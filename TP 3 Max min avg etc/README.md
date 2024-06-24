# 1 y 2. Crear una Base de datos en MySql llamada: TP47 y Crear una tabla llamada Autores que contenga los campos de la tabla.
```
  CREATE DATABASE TP47;
  
  USE TP47;
  
  CREATE TABLE `autores` (
    `Nombre` varchar(25) DEFAULT NULL,
    `Apellido` varchar(25) DEFAULT NULL,
    `Nacimiento` date DEFAULT NULL,
    `Nacionalidad` varchar(25) DEFAULT NULL,
    `Mejor_Obra` varchar(100) DEFAULT NULL,
    `Año` int(11) DEFAULT NULL,
    `Edad` int(11) DEFAULT NULL
  );
```
# 3. Realizar CRUD para que la tabla tenga los siguientes datos
```
  INSERT INTO `autores` (`Nombre`, `Apellido`, `Nacimiento`, `Nacionalidad`, `Mejor_Obra`, `Año`, `Edad`) VALUES
    ('Gabriel', 'García Márquez', '1927-03-06', 'Colombiano', 'Cien años de soledad', 1967, 40),
    ('Julio', 'Cortázar', '1914-08-26', 'Argentino', 'Rayuela', 1963, 48),
    ('Mario', 'Vargas Llosa', '1936-03-28', 'Peruano', 'La ciudad y los perros', 1963, 26),
    ('Pablo', 'Neruda', '1904-07-12', 'Chileno', 'Veinte poemas de amor y una cancion desesperada', 1924, 19),
    ('Isabel', 'Alliende', '1942-08-02', 'Chilena', 'La casa de los espiritus', 1982, 40),
    ('Jorge Luis', 'Borges', '1899-08-24', 'Argentino', 'Ficciones', 1944, 45),
    ('Octavio', 'Paz', '1914-03-31', 'Mexicano', 'El laberitno de la soledad', 1950, 36),
    ('Clarice', 'Lispector', '1920-12-10', 'Brasileña', 'La hora de la estrella', 1977, 56),
    ('Juan', 'Ruifo', '1917-05-16', 'Mexicano', 'Pedro Paramo', 1955, 38),
    ('Carlos', 'Fuentes', '1928-11-11', 'Mexicano', 'La región más transparente', 1958, 29),
    ('Eduardo', 'Galeano', '1940-09-03', 'Uruguayo', 'Las venas abiertas de América Latina', 1971, 31);
```
# 4. Realizar las siguientes consultas.
  # a. Listar todos los autores de que sean de Nacionalidad Argentina
  ```
    SELECT * FROM Autores WHERE Nacionalidad = 'Argentina' OR Nacionalidad = 'Argentino';
  ```
  # b. Listar todos los autores que tengan hayan publicado entre 1960 a 1980.
  ```
    SELECT * FROM Autores WHERE Fecha_publicacion BETWEEN '1960-01-01' AND '1980-12-31';
  ```
  # c. Mostrar el promedio de la edad de publicación. (avg).
  ```
    SELECT AVG(Edad) AS Promedio FROM Autores;
  ```
