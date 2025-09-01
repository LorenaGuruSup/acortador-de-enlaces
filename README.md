📄 README - Link Shortener MVP
Descripción

Aplicación web sencilla para generar enlaces cortos a partir de URLs largas. El objetivo del MVP es permitir a cualquier usuario ingresar un enlace, obtener una versión reducida y que este redireccione correctamente al destino original.

Características principales (MVP)

Generar un enlace corto único a partir de una URL válida.

Guardar la relación entre URL larga y URL corta en una base de datos.

Redirigir a la URL original cuando se accede al enlace corto.

Contar los clics de cada enlace.

Exponer una API REST básica para crear y acceder a enlaces.

Requisitos

Backend: Node.js (Express) o Python (FastAPI/Flask).

Base de datos: SQLite o PostgreSQL.

Cliente opcional: formulario web simple con campo de entrada para la URL.

Docker para despliegue rápido.

Tareas para el MVP
Backend

Endpoint POST /shorten que reciba una URL y devuelva un enlace corto.

Endpoint GET /:id que redirija a la URL original.

Validación de URLs (rechazar inválidas).

Persistencia en base de datos (id → url, contador de clics, fecha de creación).

Registro automático de cada clic en el enlace corto.

Frontend (opcional para MVP)

Formulario con input para pegar URL.

Mostrar enlace corto generado.

Página simple de error para enlaces no encontrados.

Infraestructura

Configuración de entorno (.env con puerto, base de datos).

Dockerfile para levantar la app fácilmente.

Tests básicos (crear enlace, redirigir, contador de clics).

Documentación mínima en README.

Futuras mejoras (post-MVP)

Autenticación de usuarios para gestionar sus enlaces.

Expiración de enlaces.

Estadísticas avanzadas (por fecha, geolocalización, navegador).

UI más robusta con panel de administración.
