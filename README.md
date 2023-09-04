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

4- Visualizar las Bases de datos creadas:

```bash
\c + TAB
```

5- Conectarse a la Base de datos, agregando su nombre:

```bash
\c tienda;
```

6- Crear tabla Usuarios con campos Nombre y Edad:

```bash
CREATE TABLE productos (id SERIAL PRIMARY KEY, nombre VARCHAR(100), precio NUMERIC(10,2), stock INT);
```

7- Visualizar tabla creada:

```bash
\dt
```

8- Insertar datos en la tabla:

```bash
INSERT INTO productos(nombre, precio, stock) VALUES('Camisetas', 19.99, 100), ('Pantalon', 99.00, 59), ('Zapatos', 50.99, 38);
```

9- Visualizar contenido de la tabla usuarios:

```bash
SELECT * FROM usuarios;
```

10- Editar tabla usuarios, agregando llave primaria

```bash
DELETE FROM usuarios;

ALTER TABLE usuarios ADD COLUMN ID INT PRIMARY KEY;
```

11- Ver datos de usuarios 

```bash
\d usuarios
```

12- Insertar id

```bash
INSERT INTO usuarios (id, nombre, edad) VALUES (1, 'Francisco', 27);
```

13- Cambiar nombre de la columna id

```bash
ALTER TABLE usuarios RENAME COLUMN id to usuario_id;
```

14- Crear tabla notas referenciada a tabla usuario, mediante columna usuario_id (foreign key)

```bash
CREATE TABLE notas (notas_id INT, nota INT, usuario_id INT REFERENCES usuarios(usuario_id));
```

15- Insertar valores en la tabla nota

```bash
INSERT INTO notas VALUES (1, 10, 1);
```






