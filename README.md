
# Biblioteca 

Un sistema de gestión de biblioteca desarrollado con Spring Boot que permite a los usuarios registrarse, iniciar sesión y realizar operaciones específicas según su rol (usuario normal o administrador).

## Funcionalidades

### Usuarios

- **Registro:** Los usuarios pueden registrarse en la aplicación proporcionando información básica.
- **Inicio de Sesión:** Los usuarios pueden iniciar sesión con sus credenciales.

### Roles

- **Usuario Normal:** Puede prestar y devolver libros.
- **Usuario Administrador:** Puede crear, eliminar libros y cambiar su estado a "en reparación".

### Libros

- **Crear Libros:** Solo el usuario administrador puede crear nuevos libros.
- **Eliminar Libros:** Solo el usuario administrador puede eliminar libros existentes.
- **Cambiar Estado de Libros:** Solo el usuario administrador puede cambiar el estado de un libro a "en reparación".

### Préstamos

- **Préstamo de Libros:** Los usuarios normales pueden tomar prestados libros por un máximo de 7 días.
- **Devolución de Libros:** Los usuarios normales pueden devolver libros.
- **Multa por Retraso:** Si un libro se devuelve después de la fecha límite, se aplica una multa (el doble de días de retraso).
- **Restricción de Préstamo con Multa:** Mientras haya una multa activa, el usuario no puede tomar prestados más libros.

## Instalación

1. Clona este repositorio.
2. Configura la base de datos en `application.properties`.
3. Ejecuta la aplicación.

## Tecnologías Utilizadas

- Spring Boot
- Spring Security
- Spring Data JPA
- Thymeleaf (o tu motor de plantillas preferido)

## Uso

1. Regístrate o inicia sesión.
2. Explora la lista de libros disponibles.
3. Realiza operaciones según tu rol: préstamo, devolución, etc.

## Contribución

1. Haz un fork del repositorio.
2. Crea una nueva rama: `git checkout -b feature/nueva-funcionalidad`.
3. Realiza tus cambios y commitea: `git commit -am 'Añade nueva funcionalidad'`.
4. Haz push a la rama: `git push origin feature/nueva-funcionalidad`.
5. Crea un pull request.

## Licencia

Este proyecto está bajo la [Licencia MIT](LICENSE).
