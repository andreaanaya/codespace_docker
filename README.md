# Introducción a Docker 🐳

Este repositorio contiene una introducción práctica al uso de Docker, una plataforma para desarrollar, enviar y ejecutar aplicaciones dentro de contenedores. Docker permite empaquetar software con todas sus dependencias en una unidad estándar para su desarrollo y despliegue ágil.

## ¿Qué es Docker?

Docker es una herramienta que permite crear y gestionar **contenedores**, que son entornos ligeros y portables. A diferencia de las máquinas virtuales, los contenedores comparten el mismo kernel del sistema operativo, lo que los hace más eficientes.

## ¿Por qué usar Docker?

- **Portabilidad**: Corre en cualquier sistema con Docker instalado.
- **Aislamiento**: Cada contenedor tiene su propio entorno.
- **Escalabilidad**: Fácil de usar en sistemas de orquestación como Kubernetes.
- **Consistencia**: El mismo entorno en desarrollo, prueba y producción.

## Requisitos

- [Docker instalado](https://docs.docker.com/get-docker/)
- Acceso a terminal o consola de comandos

## Comandos básicos de Docker

```bash
# Verifica que Docker esté instalado
docker --version

# Construye una imagen desde un Dockerfile
docker build -t nombre-imagen .

# Lista las imágenes disponibles
docker images

# Corre un contenedor desde una imagen
docker run -d -p 8000:8000 nombre-imagen

# Lista los contenedores activos
docker ps

# Detiene un contenedor
docker stop <container_id>

# Elimina un contenedor
docker rm <container_id>
