
Usando Dockerfile

# 1) Construir la imagen (elige un nombre y tag)

docker build [opciones] -t <nombre[:tag]> <contexto>

Ejemplo: docker build -t prueba1:1.0 .

# 2) Verificar que existe

docker images

# 3) Correr el contenedor

docker run [opciones] <imagen[:tag]> [comando] [args]

Ejemplo: docker run -d --name prueba1 -p 3000:3000 prueba:1.0

# 4) probar
Abrir http://localhost:3000 en el navegador

# x) Comandos
- docker ps
Lista los contenedores en ejecución en tu sistema Docker.
- docker stop [name o id]
El comando detiene un contenedor en ejecución.  
- docker start [name o id]
Esto lo vuelve a encender con la misma configuración que tenía antes.

------------------------------------------------------------

Docker compose

# 1) Levantar servicios

docker compose up -d --build

