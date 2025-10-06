# SoftDip — Sistema de Gestión de Oficios

**SoftDip** es una aplicación web desarrollada en **Django** que permite la gestión, consulta y análisis de **oficios** en el área administrativa.  
Su objetivo es **centralizar la información**, **facilitar la búsqueda de documentos** y **proveer indicadores gráficos** para la toma de decisiones.

---

##  Descripción general

SoftDip fue creado para optimizar el flujo de trabajo administrativo mediante una interfaz moderna y visual.  
Incluye autenticación por roles, dashboard estadístico, carga y visualización de oficios, y soporte para múltiples archivos PDF de respuesta por registro.

Este repositorio incluye:
- Código fuente completo del sistema.
- Documentación técnica y manual de usuario.
- Video explicativo sobre la instalación y uso de la aplicación.

---

## ⚙️ Tecnologías utilizadas

| Componente | Tecnología |
|-------------|-------------|
| **Backend** | Django 5.x (Python) |
| **Frontend** | HTML5, CSS3, Bootstrap 5, Chart.js |
| **Base de datos** | MariaDB / MySQL |
| **Librerías adicionales** | Pandas, Sklearn, BeautifulSoup, Requests, Flatpickr, Sklearn|
| **Entorno de desarrollo** | Visual Studio Code |

---

##  Funcionalidades principales

- 🔐 **Autenticación de usuarios** con roles: *Administrador* y  *Viewer*  
- 📄 **Gestión de oficios**: registro, búsqueda, filtrado y carga de archivos PDF  
- 📊 **Dashboard estadístico** con indicadores gráficos y filtros por fecha  
- 📥 **Carga múltiple de PDFs de respuesta** por oficio  
- 🤖 **Scraping** para importar datos de fuentes externas y para subir carga de PDF.   
- 🧮 **Análisis estadístico y correlacional** de oficios y respuestas

---

## Base de datos

El sistema utiliza **MariaDB** como gestor principal, con las siguientes tablas destacadas:

- `oficio`: contiene los datos generales de cada oficio (número, fecha, materia, estado, etc.)
- `pdfrespuesta`: almacena los PDFs asociados a cada oficio (relación uno a muchos)
- `usuarios`: credenciales y roles del sistema

---

## 📂 Estructura del proyecto Django

SoftDip/
-`manage.py/`
- `SoftDip/`: Configuración principal de Django
- ` oficios/`: Aplicación principal
- `models.py/ `:  Tablas de la base de datos
- `views.py/`: Lógica del sistema
- `templates/`: Vistas HTML
- `urls.py/`: Rutas
- `static/`: Archivos CSS, JS e imágenes
- `media/` : PDFs de oficios y respuestas

---

## 📹 Video explicativo
🎥 Puedes revisar el video completo de instalación, uso y recorrido de la aplicación **aquí**: **https://youtu.be/UyoBF1uiQ7c**

---

## 📑 Documentación adicional

  **Manual técnico**: explica el flujo del sistema, configuración, estructura del código y base de datos.
  **Manual de usuario**: guía paso a paso con capturas sobre cómo utilizar la aplicación.
  **Guía de instalación**: detallada para entornos con XAMPP, MariaDB y MySQL Workbench.



