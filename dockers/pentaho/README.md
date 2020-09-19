# Pentaho, Postgres y pgAdmin4

Para levantar el entorno

```docker-compose up```

Se puede acceder a Pentaho desde http://localhost:8080

 - USUARIO: admin
 - CLAVE: password

La base de datos queda en el puerto 5432.

Al pgAdmin4 se accede desde: http://localhost:9090

- USUARIO: bdm@bdm.com
- CLAVE: bdm

Para conectar la base de datos tanto desde el pgAdmin4 como desde Pentaho, se puede usar el host *pentaho_postgres*.

## Schema Workbench

Para conectar la base de datos desde el Schema Workbench, el host es *127.0.0.1* y puerto *5432*.

Para publicar un cubo a Pentaho:

 - DIRECCIÓN: http://localhost:8080/pentaho/
 - USUARIO: admin
 - CLAVE: password

**Descarga Mondrian Schema Workbench**

https://sourceforge.net/projects/mondrian/files/schema%20workbench/3.14.0/

**jre necesario para ejecutar el mondrian**

```sudo apt install default-jre```