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
   ```bash
   git clone [https://github.com/ProyectoAmpliacion/ProyectoAmpliacion.git](https://github.com/ProyectoAmpliacion/ProyectoAmpliacion.git)
   cd ProyectoAmpliacion
