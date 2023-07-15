# CRUD API USERS

¡Bienvenido/a a la API de Usuarios! Esta API te permite realizar operaciones básicas de CRUD (Crear, Leer, Actualizar, Eliminar) sobre los datos de los usuarios.

## Tecnologías Utilizadas

- Node.js
- Express.js
- UUID (para generar identificadores únicos de usuarios)

# Endpoints de la API

Obtener todos los usuarios

URL: /people

Método: GET

Descripción: Recupera una lista de todos los usuarios.

Respuesta de Ejemplo:

``[
  {
    "id": "1",
    "username": "john_doe",
    "age": 30
  },
  {
    "id": "2",
    "username": "jane_smith",
    "age": 25
  }
]``

# Crear un nuevo usuario
URL: /people

Método: POST

Descripción: Crea un nuevo usuario.

Cuerpo de la Solicitud de Ejemplo:

``{
  "username": "nuevo_usuario",
  "age": 40
}``

# Obtener un usuario específico
URL: /people/:id

Método: GET

Descripción: Recupera un usuario específico según su ID.

URL de Ejemplo: /people/1

Respuesta de Ejemplo:

``{
  "id": "1",
  "username": "john_doe",
  "age": 30
}``

# Actualizar un usuario
URL: /people/:id

Método: PATCH

Descripción: Actualiza un usuario específico según su ID.

URL de Ejemplo: /people/1

Cuerpo de la Solicitud de Ejemplo:

``{
  "username": "usuario_actualizado",
  "age": 35
}``

Eliminar un usuario
URL: /people/:id
Método: DELETE
Descripción: Elimina un usuario específico según su ID.
URL de Ejemplo: /people/1
