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

7- Insertar datos en la tabla:

```bash
INSERT INTO productos(nombre, precio, stock) VALUES('Camisetas', 19.99, 100), ('Pantalon', 99.00, 59), ('Zapatos', 50.99, 38);
```

8- Visualizar contenido de la tabla productos:

```bash
SELECT * FROM productos;
```







