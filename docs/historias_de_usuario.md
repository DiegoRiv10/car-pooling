# Historias de Usuario - Sesion 3

## Objetivo

Refinar las 4 historias de usuario principales del MVP de Car-Pooling Universitario y vincularlas con las tareas operativas creadas durante la Sesion 2.

## Formato oficial

**Como** [tipo de usuario], **quiero** [accion o necesidad], **para** [beneficio esperado].

Cada historia incluye criterios de aceptacion y subtareas sugeridas para Jira.

---

## HU-001: Registro y verificacion de usuario

**Como** estudiante universitario, **quiero** registrarme con mi correo institucional, **para** verificar que pertenezco a la comunidad universitaria y poder usar la plataforma de forma segura.

### Prioridad

Alta

### Criterios de aceptacion

- El sistema solicita nombre, correo institucional y contrasena.
- El sistema valida que el correo pertenezca a un dominio institucional permitido.
- El usuario queda en estado no verificado hasta confirmar su correo.
- El usuario no puede publicar ni solicitar viajes hasta completar la verificacion.

### Subtareas vinculadas de la Sesion 2

| ID | Subtarea |
|----|----------|
| CP-001 | Definir dominios institucionales permitidos |
| CP-002 | Crear flujo de registro con correo institucional |
| CP-003 | Disenar verificacion de cuenta por correo |
| CP-004 | Crear modelo de usuario y roles |

---

## HU-002: Publicacion de viaje

**Como** conductor universitario, **quiero** publicar un viaje con origen, destino, horario y asientos disponibles, **para** compartir mi ruta con otros estudiantes que necesiten trasladarse a la universidad.

### Prioridad

Alta

### Criterios de aceptacion

- El conductor puede capturar origen, destino, fecha, hora y numero de asientos disponibles.
- El sistema guarda el viaje asociado al usuario conductor.
- El viaje queda visible para estudiantes verificados.
- El conductor puede revisar la informacion antes de publicar.

### Subtareas vinculadas de la Sesion 2

| ID | Subtarea |
|----|----------|
| CP-005 | Definir formulario para publicar viaje |
| CP-006 | Crear modelo de viaje |
| CP-011 | Crear prototipo de pantallas principales |

---

## HU-003: Busqueda y solicitud de viaje

**Como** pasajero universitario, **quiero** buscar viajes disponibles y solicitar unirme a uno, **para** encontrar una opcion de transporte segura, economica y coordinada con otros estudiantes.

### Prioridad

Alta

### Criterios de aceptacion

- El pasajero puede buscar viajes por origen, destino y horario.
- El sistema muestra solo viajes disponibles con asientos libres.
- El pasajero puede enviar una solicitud para unirse al viaje.
- La solicitud queda registrada con estado pendiente.
- El conductor puede identificar que existe una solicitud nueva.

### Subtareas vinculadas de la Sesion 2

| ID | Subtarea |
|----|----------|
| CP-007 | Construir busqueda de viajes disponibles |
| CP-008 | Crear solicitud para unirse a un viaje |
| CP-009 | Definir estados de solicitud |
| CP-011 | Crear prototipo de pantallas principales |

---

## HU-004: Notificaciones de solicitudes y recordatorios

**Como** usuario de la plataforma, **quiero** recibir notificaciones sobre solicitudes, confirmaciones, rechazos y recordatorios de viaje, **para** mantenerme informado y coordinar mi traslado sin confusiones.

### Prioridad

Media

### Criterios de aceptacion

- El conductor recibe aviso cuando un pasajero solicita unirse a su viaje.
- El pasajero recibe aviso cuando su solicitud es aceptada o rechazada.
- El sistema puede generar recordatorios antes del horario del viaje.
- Las notificaciones muestran informacion clara sobre el viaje relacionado.

### Subtareas vinculadas de la Sesion 2

| ID | Subtarea |
|----|----------|
| CP-009 | Definir estados de solicitud |
| CP-010 | Disenar notificaciones basicas |
| CP-012 | Documentar criterios de exito del MVP |

---

## Reestructura en Jira

Las historias principales deben crearse como issues tipo **Story** en Jira. Las tareas de la Sesion 2 deben vincularse como **Subtasks** o como tareas relacionadas dentro de cada historia.

| Historia | Tareas S2 vinculadas | Responsable sugerido |
|----------|----------------------|----------------------|
| HU-001 Registro y verificacion de usuario | CP-001, CP-002, CP-003, CP-004 | Diego Quintero |
| HU-002 Publicacion de viaje | CP-005, CP-006, CP-011 | Diego Rivera |
| HU-003 Busqueda y solicitud de viaje | CP-007, CP-008, CP-009, CP-011 | Sebastian Lugo |
| HU-004 Notificaciones de solicitudes y recordatorios | CP-009, CP-010, CP-012 | Diego Quintero |

## Definicion de terminado

- Las 4 historias principales estan redactadas con el formato oficial.
- Cada historia tiene criterios de aceptacion claros.
- Las tareas de la Sesion 2 estan vinculadas como subtareas o relacionadas en Jira.
- El archivo `docs/historias_de_usuario.md` esta actualizado en el repositorio.
- Los cambios se integran a `main` mediante Pull Request.
