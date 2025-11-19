# 🌐 Hosting Template: Sitio Estático (HTML/CSS/JS)

Este repositorio contiene el código base para un sitio web estático simple, optimizado para el despliegue a través de la plataforma de Hosting.

Este template utiliza **Nginx** dentro de un contenedor Docker para servir el contenido de manera eficiente.

---

## 🚀 Cómo Empezar

Sigue estos pasos para adaptar este template a tu proyecto y desplegarlo en la plataforma de Hosting:

1.  **Clonar el Template:** Clona este repositorio a tu cuenta personal de GitHub.
2.  **Modificar el Código:**
    * Trabaja **exclusivamente** dentro de la carpeta `app/`.
    * Reemplaza el contenido de `app/index.html`, `app/style.css`, y `app/main.js` con el código de tu proyecto.
3.  **Registro en la plataforma de Hosting:**
    * Una vez que tu código esté listo en tu repositorio personal, copia la URL de dicho repositorio.
    * Regístrala en la interfaz de la plataforma de Hosting.
4.  **Despliegue:** La plataforma automáticamente construirá el contenedor y te proporcionará una URL local para acceder a tu sitio.

---

## 📁 Estructura del Template

La arquitectura está diseñada para separar tu código del proceso de despliegue.

| Archivo/Directorio | Descripción | **¿Editable por el Usuario?** |
| :--- | :--- | :--- |
| `app/` | **Contiene todo el código de tu sitio web (HTML, CSS, JS).** | ✅ SÍ |
| `app/index.html` | El archivo principal y punto de entrada de la aplicación. | ✅ SÍ |
| `app/style.css` | Hoja de estilos de la aplicación. | ✅ SÍ |
| `app/main.js` | Lógica interactiva en JavaScript. | ✅ SÍ |
| **`Dockerfile`** | **Instrucciones para Docker:** Configura el servidor Nginx y copia los archivos de la carpeta `app/`. | ❌ **NO** |

---

## ⚠️ NOTA IMPORTANTE PARA EL DESPLIEGUE

**Por favor, no modifiques el archivo `Dockerfile`** en la raíz de este repositorio. Este archivo contiene la configuración crítica necesaria para que el **Project Manager Service** de la plataforma de Hosting pueda construir y ejecutar tu contenedor correctamente con Nginx. Cualquier cambio podría provocar fallos en el despliegue.