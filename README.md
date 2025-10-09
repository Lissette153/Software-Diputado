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
- 👥 **Gestión de usuarios**: *Permite gestionar usuarios, visualización, eliminación y modificación de estos*

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
🎥 Puedes revisar el video de uso y recorrido de la aplicación **aquí**: **https://youtu.be/UyoBF1uiQ7c**
🎥 Puedes revisar el video de instalación, ejecución y guía **aquí**: **https://youtu.be/-6hMNb5nUqU**

---

## 📑 Documentación adicional

  **Manual técnico**: explica el flujo del sistema, configuración, estructura del código y base de datos.
  **Manual de usuario**: guía paso a paso con capturas sobre cómo utilizar la aplicación.
  **Guía de instalación**: detallada para entornos con XAMPP, MariaDB y MySQL Workbench.

  
## IMPORTANTE:
Para obtener los pdf de archivos se debe crear la carpeta 'media', dentro de esta, crear 'documentos' y 'respuestas_pdf'. Ya que el archivo es muy grande el de media y contiene muchos pdf. Para obtener todos los pdf de los oficios se debe ejecutar 'scraping.py',  también debe descargar manualmente las respuestas de oficio en 'respuestas_pdf' y ejecutar 'importar_pdf.py'


