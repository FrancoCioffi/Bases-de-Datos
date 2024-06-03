# 1)
```
CREATE DATABASE Restaurante;

USE Restaurante;

CREATE TABLE lista_de_comidas (
    Numero INT AUTO_INCREMENT PRIMARY KEY,
    Plato VARCHAR(25),
    Precio_porcion FLOAT
);
```
# 2)
```
INSERT INTO lista_de_comidas (Plato, Precio_porcion) VALUES
('Milanesa', 12000),
('Pizza', 15000),
('Empanadas', 8000),
('Tacos', 10000),
('Hamburguesa', 11000),
('Sushi', 25000),
('Pasta', 13000),
('Ensalada', 9000),
('Pollo al disco', 20000),
('Carne a la parrilla', 18000),
('Mariscos', 30000),
('Porcion de rabas', 14000);
```
# 3)
```
SELECT * FROM lista_de_comidas WHERE Numero = 5;
```
# 4)
```
SELECT * FROM lista_de_comidas WHERE Plato LIKE 'M%';
```
# 5)
```
SELECT * FROM lista_de_comidas WHERE Precio_porcion > 15000;
```
# 6)
```
SELECT * FROM lista_de_comidas WHERE Precio_porcion < 9000;
```
