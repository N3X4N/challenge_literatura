# Proyecto de Literatura

Este es un proyecto de ejemplo que utiliza Spring Boot para construir una aplicación web que gestiona información sobre libros y autores. La aplicación se conecta a una base de datos PostgreSQL.

## Requisitos

- Java 22.0.1
- Spring Boot 3.3.1
- PostgreSQL 14 o superior
- Maven 3.8.1 o superior

## Configuración del Entorno

1. Clona este repositorio:
    ```bash
    git clone https://github.com/tu-usuario/proyecto-literatura.git
    cd proyecto-literatura
    ```

2. Configura la base de datos PostgreSQL:
    - Crea una base de datos llamada `literatura` (o el nombre que prefieras).
    - Crea un usuario con permisos para acceder a esta base de datos.

3. Configura el archivo `.env` en el directorio raíz del proyecto con la información de la base de datos:
    ```env
    DB_HOST=localhost
    DB_PORT=5432
    DB_NAME=literatura
    DB_USER=tu_usuario
    DB_PASSWORD=tu_contraseña
    ```

## Instalación

1. Navega al directorio del proyecto y compila el proyecto con Maven:
    ```bash
    mvn clean install
    ```

2. Ejecuta la aplicación:
    ```bash
    mvn spring-boot:run
    ```

## Uso

La aplicación estará disponible en `http://localhost:8080`.

### Endpoints

- `/api/libros` - CRUD para libros.
- `/api/autores` - CRUD para autores.

## Estructura del Proyecto

