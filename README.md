# 🐳 Práctica de Docker, Portainer y Docker Compose

## 📖 Descripción

Este repositorio contiene el desarrollo de tres prácticas enfocadas en la administración de contenedores utilizando **Docker**, **Portainer** y **Docker Compose** sobre **Red Hat Enterprise Linux 10 (RHEL 10)**.

Durante las prácticas se realizó la instalación y configuración del motor de Docker, el despliegue de un servidor web NGINX con almacenamiento persistente, la administración de contenedores mediante Portainer y la implementación de un entorno completo de WordPress utilizando Docker Compose.

---

# 📌 Práctica 1 - Instalación y configuración de Docker

## Objetivos

* Instalar Docker en RHEL 10.
* Descargar la imagen oficial de NGINX desde Docker Hub.
* Crear un contenedor con redirección de puertos.
* Configurar un volumen persistente.
* Publicar una página HTML personalizada.

## Actividades realizadas

* Instalación del servicio Docker.
* Habilitación e inicio del servicio.
* Descarga de la imagen oficial de **NGINX**.
* Creación del contenedor con el puerto **8888** del host hacia el puerto **80** del contenedor.
* Creación del directorio persistente:

```
/home/website
```

* Montaje del volumen:

```
/home/website
        │
        ▼
/usr/share/nginx/html
```

* Creación del archivo **index.html** con nombre y matrícula.
* Verificación del sitio web desde:

```
http://127.0.0.1:8888
```

---

# 📌 Práctica 2 - Instalación de Portainer

## Objetivos

* Descargar la imagen oficial de Portainer.
* Implementar el contenedor.
* Administrar Docker desde una interfaz web.
* Detener el contenedor de NGINX utilizando Portainer.

## Actividades realizadas

* Descarga de la imagen de Portainer CE.
* Creación del volumen persistente para Portainer.
* Despliegue del contenedor.
* Acceso a la interfaz web mediante:

```
https://127.0.0.1:9443
```

* Vinculación con el Docker Engine local.
* Administración de contenedores.
* Detención del contenedor de NGINX desde la interfaz web.
* Verificación de que la página dejó de estar disponible.

---

# 📌 Práctica 3 - Despliegue de WordPress con Docker Compose

## Objetivos

* Instalar Docker Compose.
* Crear un archivo docker-compose.yml.
* Desplegar una base de datos MySQL/MariaDB.
* Desplegar WordPress.
* Configurar el sitio desde el navegador.

## Servicios implementados

* WordPress
* Base de datos MySQL (o MariaDB)

## Componentes definidos

* Variables de entorno
* Volúmenes persistentes
* Red interna de Docker
* Publicación de puertos
* Reinicio automático de los contenedores

## Despliegue

Los servicios fueron implementados utilizando:

```
docker compose up -d
```

Una vez iniciado el entorno se accedió desde el navegador para completar el asistente de instalación de WordPress.

---

---

# 🛠️ Tecnologías utilizadas

* Red Hat Enterprise Linux 10
* Docker Engine
* Docker Compose
* Portainer CE
* NGINX
* WordPress
* MySQL / MariaDB

---


# 📚 Competencias desarrolladas

* Administración de contenedores Docker.
* Gestión de imágenes desde Docker Hub.
* Configuración de volúmenes persistentes.
* Publicación de servicios mediante mapeo de puertos.
* Administración gráfica de contenedores con Portainer.
* Orquestación de servicios utilizando Docker Compose.
* Despliegue de aplicaciones multicontenedor.
* Implementación de un CMS (WordPress) en contenedores.

---

## 👨‍💻 Autor

**Víctor De Peña**

Tecnólogo en Seguridad Informática

Instituto Tecnológico de Las Américas (ITLA)
