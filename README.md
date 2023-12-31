![0__SjBcAbgu6sF8X5A](https://github.com/pedro-donoso/Postgresql/assets/68760595/c4386299-6604-4a21-86b9-58a66aae3d96)

# Postgresql

1- Iniciar base de datos postgresql desde terminal:

```bash
sudo service postgresql start
```

2- Iniciar psql:

```bash
sudo -u postgres psql
```

3- Crear la base de datos:

```bash
CREATE DATABASE tienda;
```

4- Conectarse a la Base de datos, agregando su nombre:

```bash
\c tienda;
```
![screen01](https://github.com/pedro-donoso/Postgresql/assets/68760595/ea4576ed-d09a-43ab-acfd-cce0760436e2)

5- Crear tabla Productos con campos Nombre y Edad:

```bash
CREATE TABLE productos (id SERIAL PRIMARY KEY, nombre VARCHAR(100), precio NUMERIC(10,2), stock INT);
```

6- Visualizar tabla creada:

```bash
\dt
```
![screen02](https://github.com/pedro-donoso/Postgresql/assets/68760595/c2fbbca0-868a-4242-9e02-3c0cbb0820a0)

7- Insertar datos en la tabla:

```bash
INSERT INTO productos(nombre, precio, stock) VALUES('Camisetas', 19.99, 100), ('Pantalon', 99.00, 59), ('Zapatos', 50.99, 38);
```

8- Visualizar contenido de la tabla productos:

```bash
SELECT * FROM productos;
```
![screen03](https://github.com/pedro-donoso/Postgresql/assets/68760595/d846fb76-5e5c-483e-980f-52adb9bec157)

9- Agregar nuevo elemento a la tabla productos:

```bash
INSERT INTO productos(nombre, precio, stock) VALUES('Camisas', 19.99, 100.5);
```
10- Ver nuevo elemento agregado a la tabla producto:

```bash
SELECT * FROM productos;
```
![screen04](https://github.com/pedro-donoso/Postgresql/assets/68760595/cc0fe3bf-6f51-453e-85ec-fad3db2c20db)

11- Consultar productos cuyo precio sea mayor a 30:

```bash
SELECT * FROM productos WHERE precio > 30;
```
![screen](https://github.com/pedro-donoso/Postgresql/assets/68760595/16721db3-a1fb-4fe0-9f3d-b9e0b88571c4)

12- Actualizar precio del producto Camisas:

```bash
UPDATE productos SET precio = 99.99 WHERE id = 4;
```
13- Ver precio actualizado del producto Camisas:

![screen01](https://github.com/pedro-donoso/Postgresql/assets/68760595/3bfa7902-f811-42e8-87bc-8974638c6923)











