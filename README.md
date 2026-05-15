# Proyecto 1: Landing Page — Gabriel Manosalvas

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)

Despliegue de una **Landing Page Profesional** utilizando **Docker** y **Nginx**, desarrollado para el Proyecto 1 de la asignatura Programación Web en la Universidad de las Fuerzas Armadas - ESPE.

---

## 📝 Descripción del Proyecto

Este proyecto presenta una Landing Page moderna y responsiva de **Gabriel Alexander Manosalvas Clavijo**. La aplicación ha sido empaquetada en un contenedor Docker utilizando **Nginx** como servidor web ligero, lo que garantiza que el sitio sea portable y pueda ejecutarse de manera idéntica en cualquier entorno de desarrollo o producción.

### Características Principales

- **Diseño Responsivo:** Adaptable a dispositivos móviles y tablets.
- **Arquitectura de Contenedores:** Aislado y listo para despliegue inmediato.
- **Semántica HTML5:** Estructura optimizada para accesibilidad.

---

## 📂 Estructura de Carpetas

```text
Proyecto1_Manosalvas/
├── assets/             # Recursos visuales (iconos, imágenes)
├── css/                # Estilos personalizados (styles.css)
├── index.html          # Estructura principal de la Landing Page
├── Dockerfile          # Configuración de la imagen Docker
├── .dockerignore       # Archivos excluidos del contenedor
├── .gitignore          # Archivos excluidos de Git
└── README.md           # Documentación técnica
```

---

## Instrucciones de Uso con Docker

### 1. Construir la imagen localmente

Si deseas realizar cambios y probarlos, construye la imagen desde el `Dockerfile`:

```bash
git clone https://github.com/GabrielManosalvas/Proyecto-1.git
cd Proyecto-1
docker build -t gamanosalvas/landing-page:v1 .
```

### 2. Ejecutar el contenedor

Ejecuta el contenedor mapeando el puerto 80 del contenedor al puerto 8080 de tu máquina:

```bash
docker run -d -p 8080:80 --name servidor-landing gamanosalvas/landing-page:v1
```

### 3. Acceder al sitio

Abre tu navegador y dirígete a:

```
http://localhost:8080
```

---

## Imagen en Docker Hub

La imagen está publicada y disponible para despliegue inmediato:

🔗 **URL:** `https://hub.docker.com/r/gamanosalvas/landing-page`

### Descargar la imagen

```bash
docker pull gamanosalvas/landing-page:v1
```

### Ejecutar directamente desde Docker Hub

Sin necesidad de clonar el repositorio, puedes ejecutar el contenedor directamente:

```bash
docker run -d -p 8080:80 --name servidor-landing gamanosalvas/landing-page:v1
```

Luego accede en tu navegador a: **http://localhost:8080**

---

## Tecnologías Utilizadas

| Tecnología | Uso |
|---|---|
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) HTML5 | Maquetación y estructura semántica |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) CSS3 | Diseño visual, variables y responsive design |
| ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) Docker | Contenerización de la aplicación |
| ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white) Nginx | Servidor web de alto rendimiento |

---

## Autor

**Gabriel Alexander Manosalvas Clavijo**  
Estudiante de Ingeniería de Software — ESPE  
🔗 [github.com/GabrielManosalvas](https://github.com/GabrielManosalvas)
