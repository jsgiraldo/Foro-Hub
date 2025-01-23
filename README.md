# Challenge ONE | Back End | Foro Alura

Bienvenido a mi solución para el último reto del programa ONE en Backend con Java y Spring. Este proyecto es una réplica del backend del foro de Alura Latam, donde estudiantes pueden interactuar, hacer preguntas y colaborar entre sí y con los profesores.

## Descripción del Proyecto

El objetivo de este proyecto es crear una API REST que permita gestionar publicaciones, usuarios y sus interacciones en un entorno de foro. Los estudiantes pueden registrar cuentas, hacer publicaciones y responder a las dudas de otros, fomentando así un ambiente de aprendizaje colaborativo.

## Requerimientos

La API REST cumple con los siguientes requerimientos:

- ✅ Crear, mostrar, actualizar y eliminar publicaciones.
- ✅ Registro e inicio de sesión de usuarios.
- ✅ Gestión de contraseñas encriptadas utilizando BCrypt.
- ✅ Cambio de contraseña y asignación de roles a usuarios.
- ✅ Autenticación mediante JSON Web Tokens (JWT).
- ✅ Autorización basada en roles.
- ✅ Implementación de Refresh Tokens.
- ✅ Manejo de excepciones con mensajes personalizados.

### Tecnologías Utilizadas

- [Eclipse](https://www.eclipse.org/)
- [H2 Database](https://www.h2database.com/)
- [MySQL](https://www.mysql.com/)
- [Java 17](https://www.java.com/en/)
- [Spring Security 6](https://start.spring.io/)
- [JSON Web Tokens (JWT)](https://jwt.io/)

## Endpoints

### Autenticación

- [Registro de usuario (Sign up)](#registro-de-usuario-sign-up)
- [Ingreso de usuario (Login)](#ingreso-de-usuario-login)
- [Salida de usuario (Log out)](#salida-de-usuario-log-out)
- [Refresh Token](#refresh-token)
- [Cambio de contraseña](#cambiar-contraseña)
- [Asignar rol a usuario](#asignar-rol-a-usuario)

### Gestión de Roles

- [Crear rol](#crear-rol)

### Gestión de Etiquetas

- [Crear Etiqueta](#crear-etiqueta)

### Gestión de Categorías y Subcategorías

- [Crear Categoría](#crear-categoría)
- [Listar Categorías](#listar-categorías)

### Publicaciones y Respuestas

- [Crear Publicación](#crear-publicacion)
- [Listar Publicaciones](#listar-publicaciones)
- [Crear Respuesta](#crear-respuesta)

## Autenticación

Para acceder a ciertos endpoints, se requiere autenticación mediante bearer token. Primero, regístrate e inicia sesión para recibir un **access token** y un **refresh token**.

- **Access Token**: JWT de corta duración que se envía en el header de las peticiones.
- **Refresh Token**: Token de mayor duración que permite generar nuevos access tokens sin necesidad de iniciar sesión nuevamente.

### Ejemplo de Uso

#### Registro de usuario (Sign up)

```bash
POST https://localhost:8080/api/v1/auth/signup
```
```json
{
  "nombre": "Fulano De Tal",
  "correo": "fulano.detal@correo.com",
  "contrasena": "admin1234"
}
```

### Cambios Realizados
- **Estructura**: Se mejoró la organización y se añadieron secciones para facilitar la navegación.
- **Descripción**: Se hizo más personal y directa, resaltando el propósito del proyecto.
- **Ejemplos**: Se incluyeron ejemplos de uso para que los usuarios comprendan mejor cómo interactuar con la API.
- **Claridad**: Se mejoró la redacción para que sea más clara y profesional.

Si necesitas más ajustes o detalles específicos, ¡házmelo saber!
