# Microservicio de Usuarios · Plazoleta de Comidas

API encargada del registro de cuentas (propietarios, empleados y clientes) y de la autenticación
de la plazoleta de comidas. Proyecto educativo construido con Spring Boot y arquitectura hexagonal;
cubre las historias de usuario HU1 a HU9 del reto.

## Requisitos

- JDK 17
- MySQL 8 (contenedor Docker recomendado)
- Maven 3.9 o superior

## Variables de entorno

| Variable | Uso |
|---|---|
| `DB_URL` | Cadena JDBC hacia la base de datos `plazoleta_usuarios` |
| `DB_USERNAME` | Usuario de la base de datos |
| `DB_PASSWORD` | Clave de la base de datos |
| `APP_JWT_SECRET` | Secreto compartido con el microservicio de restaurantes (mínimo 32 caracteres) |
| `APP_JWT_MINUTOS` | Opcional: validez del token en minutos (por defecto 480) |

## Ejecución

```bash
mvn spring-boot:run
```

## Documentación interactiva

Swagger UI disponible en: `http://localhost:8080/swagger-ui/index.html`

## Pruebas

```bash
mvn test
```
