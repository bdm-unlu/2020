# Apache Drill y MySQL

Para levantar el entorno

```docker-compose up```

Se puede acceder a Drill desde http://localhost:8047

La base de datos queda en el puerto 6603.

Al phpMyAdmin se accede desde: http://localhost:6060

- USUARIO: root
- CLAVE: bdm

## Ejemplo de conexión a MySQL

```
{
  "type": "jdbc",
  "driver": "com.mysql.jdbc.Driver",
  "url": "jdbc:mysql://drill_mysql:3306",
  "username": "root",
  "password": "bdm",
  "caseInsensitiveTableNames": false,
  "sourceParameters": {},
  "enabled": true
}
```