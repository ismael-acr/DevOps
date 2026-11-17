# Proyecto Unidad 1 - DevOps

Formulario web para reserva de horas medicas desplegado mediante contenedores.

## Archivos de configuracion raiz

- Dockerfile: Construccion del contenedor basado en la imagen ligera nginx:alpine.
- docker-compose.yml: Configuracion y orquestacion, exponiendo el servicio en el puerto 8080.
- .gitignore: Exclusiones de archivos temporales y locales para el control de versiones.
- .env.example: Archivo de ejemplo para la definicion de variables de entorno.
- README.md: Documentacion del proyecto e instrucciones de ejecucion.

## Instrucciones de ejecucion

Requisitos: Tener Git y Docker Desktop instalados y en ejecucion en el equipo local.

Clonar el repositorio y acceder a la carpeta del proyecto:
git clone https://github.com/ismael-acr/DevOps.git
cd DevOps/ProyectoUnidad1

Levantar el servicio en Docker:
docker compose up -d --build

Revisar la aplicacion funcionando en el navegador:
http://localhost:8080

Detener el servicio y limpiar los contenedores:
docker compose down