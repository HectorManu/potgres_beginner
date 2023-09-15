# Guía en español para iniciantes de Postgres en Ubuntu 

## Instalación

```bash
sudo apt install postgresql postgresql-contrib
```

## Inicio en postgres

```bash
sudo su - postgres
```

Una vez dentro de el superusuario: 

```bash
psql
```

### Creando un usuario 

```bash
create user CAMBIA_NOMBRE_DEL_USUARIO with password 'password_of_user'
```

## Creando la primera base datos

Insetamos en terminal 

```bash
sudo -u postgres psql
```

Una vez dentro de postgres sql ejecutamos el siguiente comando para observar las bases de datos que hay: 

```psql
\l
```

Crea tú primera base de datos con el usuario que diste anteriormente:
```bash
CREATE DATABASE "TuBaseDeDatos" WITH OWNER = "TuUsuario";
```

Accerde a la base de datos: 

```bash
psql -U owner_of_database -d name_of_database
```




