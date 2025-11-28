Este proyecto contiene pruebas automatizadas para el endpoint de Crear Kit de la aplicación Urban Grocers.
Las pruebas revisan cómo funciona el campo name cuando se crea un kit para un usuario.

Archivos del proyecto

configuration.py → Contiene la URL del servidor y las rutas de la API.

data.py → Cuerpos base de las solicitudes.

sender_stand_request.py → Funciones que envían solicitudes a la API.

create_kit_name_kit_test.py → Todas las pruebas del campo name.

README.md → Este archivo.

.gitignore → Para evitar subir archivos innecesarios.

Cómo ejecutar el proyecto

Clonar el repositorio:

git clone git@github.com:TU-USUARIO/qa-project-Urban-Grocers-app-es.git


Instalar las librerías necesarias:

pip install pytest requests


Iniciar el servidor en TripleTen y copiar la URL en configuration.py.

Ejecutar las pruebas:

pytest

Qué prueban los tests

Las pruebas revisan diferentes valores para el campo name del kit:

1 caracter

511 caracteres

0 caracteres (debe dar error)

512 caracteres (debe dar error)

Caracteres especiales

Espacios

Números

Falta del parámetro

Tipo incorrecto (número en vez de texto)

Las pruebas exitosas deben devolver código 201, las negativas 400.

Tecnologías usadas

Python

Requests

Pytest
