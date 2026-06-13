# Arquitectura de Datos - Sesion 4

## Objetivo

Documentar el escaneo de dos pantallas clave del MVP y definir que estructura de datos viaja desde la interfaz hacia el servidor.

## Pantallas seleccionadas

| Pantalla | Historia MVP | Archivo JSON | Metodo HTTP | Endpoint sugerido |
|----------|--------------|--------------|-------------|-------------------|
| Registro y verificacion de usuario | HU-001 | `registro_usuario.json` | POST | `/api/v1/auth/register` |
| Busqueda de viajes disponibles | HU-003 | `busqueda_viajes.json` | GET | `/api/v1/rides` |

## Justificacion HTTP basada en Swagger

### Registro y verificacion de usuario - POST

La pantalla de registro debe usar **POST** porque envia un cuerpo JSON al servidor para crear un nuevo recurso: la cuenta del usuario. En Swagger/OpenAPI, este caso se modela como una operacion `post` con `requestBody`, porque la informacion viaja en el cuerpo de la peticion.

Archivo relacionado:

- `registro_usuario.json`

Ejemplo conceptual:

```http
POST /api/v1/auth/register
Content-Type: application/json
```

### Busqueda de viajes disponibles - GET

La pantalla de busqueda debe usar **GET** porque consulta informacion existente sin crear ni modificar recursos. En Swagger/OpenAPI, este caso se modela como una operacion `get` con parametros de consulta (`query parameters`) como origen, destino, fecha y horario.

Archivo relacionado:

- `busqueda_viajes.json`

Ejemplo conceptual:

```http
GET /api/v1/rides?origin=Zona%20Rio&destination=CESUN%20Universidad&departure_date=2026-06-13
```

## Escaneo de campos por pantalla

### Registro y verificacion de usuario

- Campo de texto: Nombre_Completo
- Campo de texto/email: Correo_Institucional
- Campo de texto: Matricula
- Campo de password: Contrasena
- Campo de password: Confirmar_Contrasena
- Selector: Rol_Usuario
- Booleano/Check: Acepta_Terminos

### Busqueda de viajes disponibles

- Campo de texto: Origen
- Campo de texto: Destino
- Selector de fecha: Fecha_Salida
- Selector de hora: Hora_Inicio
- Selector de hora: Hora_Fin
- Campo numerico: Asientos_Requeridos
- Booleano/Check: Solo_Disponibles
- Selector: Ordenar_Por

## Relacion con Jira

Para esta sesion, las tareas pasadas de diseno deben moverse a **Done**. El nuevo paquete tecnico debe iniciar en **In Progress**.

Tareas tecnicas sugeridas:

| Tarea | Estado sugerido | Relacion |
|-------|-----------------|----------|
| Escanear pantalla de registro | In Progress | HU-001 |
| Crear `registro_usuario.json` | In Progress | HU-001 |
| Escanear pantalla de busqueda de viajes | In Progress | HU-003 |
| Crear `busqueda_viajes.json` | In Progress | HU-003 |
| Documentar metodos HTTP en arquitectura | In Progress | HU-001 / HU-003 |

## Definicion de terminado

- Existen dos archivos `.json`, uno por cada pantalla principal.
- Cada JSON mapea campos de interfaz, tipos de dato, validaciones y respuesta esperada.
- El README de arquitectura documenta el metodo HTTP correspondiente a cada pantalla.
- Los cambios se integran a `main` mediante Pull Request.
