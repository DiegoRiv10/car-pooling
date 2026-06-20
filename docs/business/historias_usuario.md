# Historias de Usuario y Criterios Gherkin

## Proyecto

Car-Pooling Universitario

## Objetivo

Documentar las historias de usuario principales del MVP con criterios de aceptacion en formato Gherkin: **Dado / Cuando / Entonces**.

---

## HU-001: Registro y verificacion de usuario

**Como** estudiante universitario, **quiero** registrarme con mi correo institucional, **para** verificar que pertenezco a la comunidad universitaria y poder usar la plataforma de forma segura.

### Criterios de aceptacion

```gherkin
Escenario: Registro con correo institucional valido
  Dado que el estudiante se encuentra en la pantalla de registro
  Cuando captura nombre, correo institucional, contrasena y acepta terminos
  Entonces el sistema crea una cuenta pendiente de verificacion
```

```gherkin
Escenario: Registro con dominio no institucional
  Dado que el estudiante se encuentra en la pantalla de registro
  Cuando captura un correo con dominio no permitido
  Entonces el sistema rechaza el registro y muestra un mensaje de validacion
```

```gherkin
Escenario: Acceso bloqueado sin verificacion
  Dado que el estudiante ya creo su cuenta pero no verifico su correo
  Cuando intenta publicar o solicitar un viaje
  Entonces el sistema bloquea la accion hasta completar la verificacion
```

---

## HU-002: Publicacion de viaje

**Como** conductor universitario, **quiero** publicar un viaje con origen, destino, horario y asientos disponibles, **para** compartir mi ruta con otros estudiantes que necesiten trasladarse a la universidad.

### Criterios de aceptacion

```gherkin
Escenario: Publicar viaje con datos completos
  Dado que el conductor tiene una cuenta verificada
  Cuando captura origen, destino, fecha, hora y asientos disponibles
  Entonces el sistema publica el viaje como disponible
```

```gherkin
Escenario: Intento de publicar viaje incompleto
  Dado que el conductor esta en el formulario de publicacion
  Cuando deja campos obligatorios vacios
  Entonces el sistema muestra errores y no publica el viaje
```

```gherkin
Escenario: Revisar viaje antes de publicarlo
  Dado que el conductor completo la informacion del viaje
  Cuando selecciona la opcion de revisar
  Entonces el sistema muestra un resumen con ruta, horario y cupos antes de confirmar
```

---

## HU-003: Busqueda y solicitud de viaje

**Como** pasajero universitario, **quiero** buscar viajes disponibles y solicitar unirme a uno, **para** encontrar una opcion de transporte segura, economica y coordinada con otros estudiantes.

### Criterios de aceptacion

```gherkin
Escenario: Buscar viajes disponibles
  Dado que el pasajero tiene una cuenta verificada
  Cuando ingresa origen, destino y fecha de salida
  Entonces el sistema muestra viajes activos con asientos disponibles
```

```gherkin
Escenario: Solicitar lugar en un viaje
  Dado que el pasajero visualiza el detalle de un viaje disponible
  Cuando selecciona solicitar lugar
  Entonces el sistema crea una solicitud con estado pendiente
```

```gherkin
Escenario: Busqueda sin resultados
  Dado que el pasajero captura filtros de busqueda validos
  Cuando no existen viajes disponibles para esa ruta y fecha
  Entonces el sistema muestra un mensaje indicando que no hay resultados
```

---

## HU-004: Notificaciones de solicitudes y recordatorios

**Como** usuario de la plataforma, **quiero** recibir notificaciones sobre solicitudes, confirmaciones, rechazos y recordatorios de viaje, **para** mantenerme informado y coordinar mi traslado sin confusiones.

### Criterios de aceptacion

```gherkin
Escenario: Notificar nueva solicitud al conductor
  Dado que un pasajero solicita unirse a un viaje
  Cuando la solicitud queda registrada
  Entonces el conductor recibe una notificacion con el detalle del viaje
```

```gherkin
Escenario: Notificar respuesta al pasajero
  Dado que el conductor revisa una solicitud pendiente
  Cuando acepta o rechaza la solicitud
  Entonces el pasajero recibe una notificacion con la respuesta
```

```gherkin
Escenario: Enviar recordatorio de viaje
  Dado que un viaje confirmado esta proximo a iniciar
  Cuando se alcanza el tiempo configurado de recordatorio
  Entonces el sistema notifica a conductor y pasajero con la informacion del viaje
```

---

## Trazabilidad

| Historia | Diseno relacionado | Contrato JSON relacionado |
|----------|--------------------|---------------------------|
| HU-001 Registro y verificacion de usuario | Login / Registro en Figma | `docs/architecture/contratos/registro_usuario.json` |
| HU-002 Publicacion de viaje | Home / Publicar viaje en Figma | No requerido en esta iteracion de contratos |
| HU-003 Busqueda y solicitud de viaje | Busqueda de viajes en Figma | `docs/architecture/contratos/busqueda_viajes.json` |
| HU-004 Notificaciones de solicitudes y recordatorios | Home / Notificaciones en Figma | No requerido en esta iteracion de contratos |
