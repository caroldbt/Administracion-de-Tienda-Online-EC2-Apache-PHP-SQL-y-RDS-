# Administración de TiendaOnline EC2 - Apache - PHP SQL y RDS

## Verifica la configuración del servidor Apache
- Asegúrate de configurar adecuadamente los ajustes de seguridad ( permitir el tráfico HTTP, SSH) ademas de los puertos 3036 y 8080.
## Crear RDS
## Crear tabla  en RDS
- Conectarse a la base de datos:
- Inicia el servidor MySQL en sistema Linux utilizando systemctl.
- Configura el servicio MySQL para que se inicie automáticamente cada vez que el sistema se inicie.
- Inicie una sesión interactiva de MySQL con el usuario "admin" en el servidor MySQL especificado. Una vez que ingresas la contraseña del usuario, tendrás acceso a la consola de MySQL donde puedes ejecutar consultas y comandos de administración de bases de datos.
- Una vez conectado Crea la base de datos y la tabla necesarios:
1. CREATE DATABASE IF NOT EXISTS your_database_name;
2. USE your_database_name;
3. CREATE TABLE IF NOT EXISTS your_table_name (
4. id INT AUTO_INCREMENT PRIMARY KEY,
5. nombre VARCHAR(255) NOT NULL,
6. precio DECIMAL(10,2) NOT NULL, );

- Debe examinar el contenido de los archivos (agregar, borrar, index, modificar) y cambiar el nombre del servidor por el endpoint de la RDS.
- Cambiar el nombre de usuario, password y la base de datos.
- Asegurese de que la tabla obtenga el nombre adecuado.
- Una vez realizado los cambios, probar la applicación en el explorador.
