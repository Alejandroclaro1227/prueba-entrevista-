Diagrama de Arquitectura - Planificación


Para este sistema de reservas, propongo una arquitectura basada en:

Frontend: Aplicación web React que permita realizar, modificar, cancelar y visualizar reservas.
Backend: API RESTful en Django para gestionar las reservas y usuarios.
Base de Datos: PostgreSQL para gestionar las relaciones entre usuarios, reservas y servicios.
Autenticación: JWT para proteger las rutas de la API que gestionan reservas.





+-----------------------+              +------------------+
|   Frontend (React)     | <--------->  |  Backend (Django)|
+-----------------------+              +------------------+
        |                                         |
        v                                         v
+-----------------------+              +------------------+
|    API REST (Django)   |              |    DB (Postgres) |
+-----------------------+              +------------------+





