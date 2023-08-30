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
CREATE DATABASE integridad_referencial;
```

4- Visualizar las Bases de datos creadas:

```bash
\c + TAB
```

5- Conectarse a la Base de datos, agregando su nombre:

```bash
\c integridad_referencial;
```

6- Crear tabla Usuarios con campos Nombre y Edad:

```bash
CREATE TABLE usuarios (nombre VARCHAR(50), edad INT);
```

7- Visualizar tabla creada:

```bash
\dt
```

8- Insertar datos en la tabla:

```bash
INSERT INTO usuarios(nombre, edad) VALUES('Consuelo', 27);
```

9- Visualizar contenido de la tabla usuarios:

```bash
SELECT * FROM usuarios;
```




