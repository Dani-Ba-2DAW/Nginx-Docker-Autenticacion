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

## Tarea 3

¡Importante: Cambia la IP de la configuración por la de tu anfitrión!
### 3.1 - Restricción por IP

#### Configuración
![Imagen de tarea 3.1 configuración](./img/007.png)

#### Error
![Imagen de tarea 3.1 error](./img/008.png)

### 3.2 - Restricción por IP y Usuario
¡El punto explicado en el apartado 2.3 es más o menos lo mismo que esto!

#### Configuración
![Imagen de tarea 3.2 configuración](./img/009.png)

#### Acceso sin problemas
![Imagen de tarea 3.2 acceso](./img/010.png)