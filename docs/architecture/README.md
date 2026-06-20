# Arquitectura de Datos y Metodos HTTP

## Objetivo

Explicar los contratos JSON que modelan los datos que viajan desde las pantallas clave del MVP hacia el servidor, siguiendo el criterio visto en Swagger/OpenAPI.

## Contratos incluidos

| Pantalla | Historia relacionada | Contrato JSON | Metodo HTTP | Endpoint sugerido |
|----------|----------------------|---------------|-------------|-------------------|
| Registro y verificacion de usuario | HU-001 | `contratos/registro_usuario.json` | POST | `/api/v1/auth/register` |
| Busqueda de viajes disponibles | HU-003 | `contratos/busqueda_viajes.json` | GET | `/api/v1/rides` |

## Justificacion por metodo HTTP

### Registro y verificacion de usuario - POST

La pantalla de registro utiliza **POST** porque envia informacion nueva al servidor para crear una cuenta de usuario. En Swagger/OpenAPI, esta operacion se documenta con `requestBody`, ya que los campos del formulario viajan dentro del cuerpo de la peticion.

Campos principales:

- Nombre completo
- Correo institucional
- Matricula
- Contrasena
- Confirmacion de contrasena
- Rol de usuario
- Aceptacion de terminos

### Busqueda de viajes disponibles - GET

La pantalla de busqueda utiliza **GET** porque consulta recursos existentes sin modificarlos. En Swagger/OpenAPI, esta operacion se documenta con parametros de consulta (`query parameters`) como origen, destino, fecha, horario y asientos requeridos.

Campos principales:

- Origen
- Destino
- Fecha de salida
- Hora de inicio
- Hora de fin
- Asientos requeridos
- Solo disponibles
- Ordenamiento

## Relacion con Figma

Los contratos JSON coinciden con los campos visibles en las pantallas de Figma y en los wireframes de `docs/design/`.

- Login / Registro -> `contratos/registro_usuario.json`
- Busqueda de viajes -> `contratos/busqueda_viajes.json`

## Validacion tecnica

Ambos archivos JSON deben mantenerse con formato valido, tipos de dato claros, campos requeridos y respuestas esperadas del servidor.
