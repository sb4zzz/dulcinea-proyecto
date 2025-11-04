🎵 Proyecto Dulcinea - Sistema de Gestión Musical

Aplicación web desarrollada en Flask (Python) para la gestión de artistas, bandas, solistas, álbumes, canciones, disqueras y contratos musicales.  
El sistema permite registrar, consultar, actualizar y eliminar información mediante una interfaz web conectada a un backend alojado en una máquina virtual Ubuntu.

Tecnologías Utilizadas:
- Sistema Operativo: Ubuntu (en VirtualBox)
- Backend: Python 3.13 con Flask
- Frontend: HTML, CSS y JavaScript
- Base de Datos: MySQL (servida por XAMPP)
- ORM: SQLAlchemy
- API: RESTful con Flask

Estructura del Proyecto:

ProyectoDulcinea/
├── Backend MV/
│ ├── app.py
│ ├── models.py
│ ├── database.py
│ └── pycache/
├── frontend/
│ ├── index.html
│ ├── script.js
│ └── styles.css
└── scripts_sql/

Implementación:
1. Configuración de la máquina virtual
   - Sistema base: Ubuntu en VirtualBox.
   - Carpeta creada: `Backend MV` para aislar el entorno de desarrollo.
   - Creación de entorno virtual:
     
     python3 -m venv venv
     source venv/bin/activate
     

2. Instalación de dependencias
   
   pip install Flask Flask-SQLAlchemy Flask-Cors SQLAlchemy PyMySQL
   
Configuración de la base de datos

Servidor MySQL corriendo en XAMPP.

Base de datos conectada al backend mediante SQLAlchemy:
mysql+pymysql://root@localhost/dulcinea_db

Ejecución del servidor Flask
flask run --host=0.0.0.0

Acceso desde el navegador

Abrir el archivo index.html directamente desde el navegador.

El frontend consume la API Flask a través de la IP de la MV.

Funcionalidades Principales:
CRUD para todas las entidades (Artistas, Álbumes, Canciones, Disqueras, Contratos).

Cálculo automático de duración total de álbum según sus canciones.

Eliminación en cascada de registros relacionados.

Comunicación entre frontend y backend mediante fetch API.

Autor
Santiago Moreno, Kevin Cortes, Sebastián Ayala
Proyecto Bases De Datos 1 - Universidad El Bosque
2025
