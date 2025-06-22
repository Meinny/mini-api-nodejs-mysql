# mini-api-nodejs-mysql

API básica desarrollada con Node.js, Express y MySQL. Permite listar y agregar usuarios.

## Tecnologías utilizadas
- Node.js
- Express
- MySQL
- Postman (para pruebas)

## Funcionalidades
- `GET /usuarios`: lista todos los usuarios desde la base de datos.
- `POST /usuarios`: agrega un nuevo usuario enviando JSON con `nombre` y `email`.

## Cómo usar

1. Clonar el repositorio:
   
git clone https://github.com/Meinny/mini-api-nodejs-mysql.git
cd mini-api-nodejs-mysql

3. Instalar dependencias:


3. Crear base de datos:

CREATE DATABASE mini_api_db;
USE mini_api_db;
CREATE TABLE usuarios (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nombre VARCHAR(100),
  email VARCHAR(100)
);

4. Ejecutar servidor
   
node index.js

5. Probar endpoints en Postman:

GET http://localhost:3000/usuarios
POST http://localhost:3000/usuarios
