# 🚀 Solución de Automatización: WebFusion Digital S.L.

Este proyecto implementa una infraestructura reproducible y automatizada para el despliegue de sitios WordPress, eliminando los procesos manuales y los errores de sincronización de versiones.

## 🎯 Objetivo
Estandarizar el entorno de desarrollo y producción mediante el uso de **Vagrant**, **Docker** y **GitHub**, permitiendo despliegues con un solo comando.

---

## 🏗️ Arquitectura del Sistema
La solución se basa en tres capas de automatización:
1.  **Virtualización (Vagrant):** Crea una VM Ubuntu con recursos optimizados (4GB RAM, 2 CPUs).
2.  **Orquestación (Docker Compose):** Gestiona los servicios de WordPress y base de datos MySQL.
3.  **Despliegue Continuo (Git Container):** Un contenedor especializado sincroniza automáticamente el código PHP desde GitHub hacia el servidor web.

---

## 🛠️ Requisitos Previos
Antes de comenzar, asegúrese de tener instalado:
* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* Un cliente de Git.

---

## 🚀 Instrucciones de Despliegue (Paso a Paso)

Para poner en marcha el entorno desde cero, siga estos comandos en su terminal:

1. **Clonar el repositorio:**
   git clone [https://github.com/ProyectoAmpliacion/ProyectoAmpliacion.git](https://github.com/ProyectoAmpliacion/ProyectoAmpliacion.git)
   cd ProyectoAmpliacion

2. **Levantar el entorno:**
   vagrant up
   
*Este comando creará la VM, instalará Docker y desplegará los contenedores automáticamente.

3. **Acceso al sitio web:**
   Una vez finalizado, abra su navegador en: http://localhost:8080


## 🔄 Actualización del Contenido (Continuous Deployment)
Para cumplir con el requisito de actualización rápida sin intervención manual:

Realice cambios en el archivo index.php dentro de este repositorio de GitHub.
En su terminal local, ejecute:

   vagrant provision
   
Los cambios se reflejarán inmediatamente en el entorno de WordPress.


## 📁 Estructura del Repositorio
Vagrantfile: Configuración de la infraestructura virtual.

docker-compose.yml: Definición de servicios (WordPress, DB y Git-Sync).

web/: Directorio vinculado al volumen de WordPress donde se aloja el código.

index.php: Página principal personalizada del proyecto.


## 👥 Equipo de Desarrollo (WebFusion)
Giulia Alisia Gherghin
Marta Pérez García
Laura Gema Moreno Llarena
   
