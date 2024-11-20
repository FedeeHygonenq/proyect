# 🏦 **Trabajo Práctico Final: Credicoop - UTN**

✨ **Descripción del Proyecto:**  
Este proyecto consiste en el despliegue y gestión de dos aplicaciones:  
- **OpenCart:** Sistema de gestión de tiendas en línea.  
- **API Libros (APPx):** Una API desarrollada con Java y Javalin.  
Ambas aplicaciones están configuradas y desplegadas utilizando herramientas modernas de infraestructura como **Docker**, **Kubernetes**, **Jenkins**, y **Ansible**.

---

## 👥 **Integrantes del Equipo**  
-----------------------------------------------------------------------------
|         Nombre           |                      Contacto                  |
|--------------------------|------------------------------------------------|
| **Federico Hygonenq**    | [GitHub](https://github.com/FedeeHygonenq)     |
| **Mercedes Cantarero**   | [GitHub](https://github.com/MMercedesCantarero)|
-----------------------------------------------------------------------------

## 📜 **Flujo de Ejecución**  

### **1. Pasos Principales**  

1. **Preparar Jenkins**:  
   - Configura las credenciales para **Docker Hub** y **GitHub** en el Administrador de Credenciales de Jenkins.  

2. **Pipeline de Jenkins**:  
   - **Git Clone/Pull**: Descarga o actualiza el repositorio.  
   - **Análisis con SonarQube**: Ejecuta pruebas de calidad y seguridad de código.  
   - **Construcción y Push de Imágenes**: Construye y sube las imágenes Docker a Docker Hub.  
   - **Despliegue en Minikube**: Usa un pipeline secundario para aplicar cambios y reiniciar despliegues.  

3. **Integración de OpenCart**:  
   - Despliega OpenCart y su base de datos MariaDB con **Docker Compose**.  
   - Configura OpenCart automáticamente con **Ansible** para facilitar la gestión.  

4. **Configuración de APPx**:  
   - Utiliza un archivo `deployment.yaml` para desplegar la API en Minikube.  
   - Usa un `configMap` para gestionar las credenciales de conexión a PostgreSQL.

### **Resultado Final**  
- OpenCart funcionando en un entorno Docker Compose.  
- API Libros desplegada y operativa en un clúster Kubernetes gestionado con Minikube.  

---

## 🎥 **Demostración en Video**  

¡Mira cómo funciona nuestro proyecto en tiempo real!  

![YouTube Image](https://yt3.googleusercontent.com/ytc/AIdro_lNJyStmT0jny2F8PNZ9aXQKNdoLAEXWq_wNSR3dMFgm88=s900-c-k-c0x00ffffff-no-rj)
[![YouTube Image](https://yt3.googleusercontent.com/ytc/AIdro_lNJyStmT0jny2F8PNZ9aXQKNdoLAEXWq_wNSR3dMFgm88=s900-c-k-c0x00ffffff-no-rj)](https://www.youtube.com/channel/UCBrGE6cmFbcwzlwAyIDMGpw)

---

## 📑 **Material Adicional**  

- **Informe del Trabajo Práctico:** [Informe.pdf](https://docs.google.com/document/d/10VJ1JLRX0kjF57elAz3tl41ZZGYNZRc9KgOWHvko8JM/edit?usp=sharing)  
- **Presentación:** [Presentación.pptx](https://docs.google.com/presentation/d/1YbpbYd14eEk4QtBp-_ZEEkWeTq_r9c1om3oVP2cRjzU/edit?usp=sharing)  
