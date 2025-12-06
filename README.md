# Autenticación en Nginx con Docker

## Instalación de paquetes necesarios
![Imagen de instalación de paquetes necesarios](./img/001.png)

### Creación de usuarios y contraseñas para el acceso web
![Imagen de creación de usuarios y contraseñas para el acceso web](./img/002.png)

### Configurando el contenedor Nginx para usar autenticación básica
![Imagen de configurando el contenedor Nginx para usar autenticación básica](./img/003.png)

### Probando la nueva configuración

¡Recuerda cambiar "~" por "C:/Users/[usuario]" si estás en Windows!<br><br>
Comando: docker run -d --name nginx-dani -p 80:80 -v ~/nginx/dani.test/html:/usr/share/nginx/html -v ~/nginx/dani.test/conf/htpasswd:/etc/nginx/.htpasswd -v ~/nginx/dani.test/conf/dani.test.conf:/etc/nginx/conf.d/default.conf nginx:latest

![Imagen de probando la nueva configuración](./img/004.png)

## Tarea 2

### 2.1 - Logs
![Imagen de tarea 2.1](./img/005.png)

### 2.2 - Restricción independiente
![Imagen de tarea 2.2](./img/006.png)