# Django - Laboratorio 04 (`proyecto_relacion_modelos`)

Aplicación web de tipo **Blog** desarrollada en **Django** para el Laboratorio 04 del curso **Desarrollo de Aplicaciones Empresariales (DAE)**. Se centra en la definición de relaciones entre modelos (`ForeignKey`), consultas filtradas por autor, herencia de plantillas HTML y gestión de archivos estáticos CSS.

## Características Principales

* **Relación de Modelos (`blog/models.py`):** Vinculación entre autores y publicaciones con historial de migraciones controladas.
* **Herencia de Plantillas:** Uso de una plantilla maestra (`base.html`) extendida por las vistas de listado general (`lista_entradas.html`) y filtrado por autor (`entradas_autor.html`).
* **Estilos Personalizados:** Integración de hojas de estilo mediante la carpeta `static/blog/css/estilos.css`.

## Estructura del Proyecto

```text
Django-Lab04-DAE/
└── proyecto_relacion_modelos/
    ├── manage.py
    ├── db.sqlite3
    ├── proyecto_relacion_modelos/  # Configuración y enrutamiento raíz
    └── blog/                       # Aplicación del blog
        ├── models.py               # Modelos Autor y Entrada
        ├── views.py                # Vistas de listado y filtro por autor
        ├── urls.py                 # Rutas de la aplicación
        ├── static/blog/css/        # Hoja de estilos estilos.css
        └── templates/blog/         # Plantillas base.html, lista_entradas.html y entradas_autor.html
```

## Instalación y Ejecución

1. Clona el repositorio:
   ```bash
   git clone https://github.com
   cd Django-Lab04-DAE
   ```
2. Crea un entorno virtual, actívalo e instala Django:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   pip install django
   ```
3. Inicia el servidor desde `proyecto_relacion_modelos`:
   ```bash
   cd proyecto_relacion_modelos
   python manage.py runserver
   ```
