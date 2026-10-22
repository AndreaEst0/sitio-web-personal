# Sitio Web de Presentación Profesional 
## Objetivo del Proyecto
Desarrollar mi sitio web de presentación personal utilizando HTML, CSS, y aplicar contenedores Docker con Nginx para empaquetarlo y subirlo a Docker Hub, asegurando que el proyecto sea portable y fácil de ejecutar en cualquier entorno.
## Tecnologías Utilizadas
- **Desarrollo Frontend:** HTML5 semántico, CSS3 externo (estilos personalizados, CSS Grid).
- **Servidor Web & Contenedorización:** Nginx (imagen base `nginx:alpine`), Docker Engine, Docker Desktop.
- **Control de Versiones y Despliegue:** Git, GitHub, Docker Hub.
## Estructura del Proyecto
- **`index.html`:** Documento principal del sitio web con la estructura HTML5 semántica y las secciones del perfil.
- **`estilos.css`:** Archivo CSS3 externo con el diseño visual definido, paleta de colores y componentes interactivos.
- **`fotocarnet.jpg`:** Recurso multimedia (fotografía de perfil) utilizado en la tarjeta del encabezado del sitio.
- **`Dockerfile`:** Script de automatización que empaqueta la aplicación usando la imagen ligera `nginx:alpine`.
- **`README.md`:** Documentación técnica que explica el objetivo, tecnologías, despliegue y enlaces del proyecto.
## Instrucciones para Construir y Ejecutar la Imagen Docker
Antes de comenzar con la construcción de la imagen Docker, se debe tener instalado Docker Desktop y tener abierta la sesión Docker Hub.
```bash
# 1. Construir la Imagen Docker
# Abre la terminal en la carpeta principal del proyecto donde se encuentra el Dockerfile y ejecuta el siguiente comando:
docker build -t tu-usuario-dockerhub/nombre-de-tu-imagen:latest 

# 2. Ejecutar el Contenedor
# Inicia el servidor Nginx exponiendo el puerto 80 del contenedor en el puerto 8080 de tu máquina:
docker run -d -p 8080:80 --name mi-contenedor tu-usuario-dockerhub/nombre-de-tu-imagen:latest

# 3. Verificar y Probar la Aplicación
# Confirma que el contenedor está activo corriendo:
docker ps

# Luego abre tu navegador web e ingresa a:
# http://localhost:8080

Y siguiendo todos estos pasos, se construye correctamente la imagen Docker.
```
## Enlace a Docker Hub
 **https://hub.docker.com/r/andre340/mi-sitio-web**
