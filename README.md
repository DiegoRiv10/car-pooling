# Car-Pooling Universitario

## Portada del Proyecto Final

| Campo | Detalle |
|-------|---------|
| Proyecto | Car-Pooling Universitario |
| Materia | Administracion de Proyectos de Software |
| Equipo | Diego Rivera, Sebastian Lugo, Diego Quintero |
| Repositorio | https://github.com/DiegoRiv10/car-pooling |
| Jira | https://cesunbc-team-ztwxd7jm.atlassian.net/jira/software/projects/CPTU/list |
| Figma publico | https://www.figma.com/design/MIRhazuP9aB3Xar4AluQd0/4.1-Sitemap--Figma---Jira?node-id=0-1&t=Gkx5SDKngm0TWZJ1-1 |

## Propuesta de Valor

Car-Pooling Universitario es una plataforma para conectar estudiantes que viajan hacia la misma universidad. El MVP permite registrar usuarios con correo institucional, publicar viajes, buscar rutas disponibles, solicitar lugares y recibir notificaciones relacionadas con el traslado.

## Alcance del MVP

1. Registro y verificacion de usuarios.
2. Publicacion de viajes por conductores.
3. Busqueda y solicitud de viajes por pasajeros.
4. Notificaciones de solicitudes, confirmaciones, rechazos y recordatorios.

## Estructura Final del Repositorio

```text
car-pooling/
├── README.md
└── docs/
    ├── business/
    │   └── historias_usuario.md
    ├── design/
    │   ├── README.md
    │   ├── sitemap.png
    │   ├── user_flows.pdf
    │   ├── wireframe_login.png
    │   ├── wireframe_home.png
    │   └── wireframe_busqueda_viajes.png
    └── architecture/
        ├── README.md
        └── contratos/
            ├── registro_usuario.json
            └── busqueda_viajes.json
```

## Entregables por Rubrica

### Gestion de Proyecto

- Tablero Jira con historias principales y subtareas.
- Sprint final cerrado en Jira.
- Historias y tareas tecnicas en estado Done.
- Comentarios de evidencia con enlaces a Figma y GitHub.

### Diseno e Interactividad

- Prototipo publico en Figma.
- Sitemap del MVP en `docs/design/sitemap.png`.
- User flows en `docs/design/user_flows.pdf`.
- Wireframes de Login, Home y Busqueda de viajes.

### Ingenieria y Documentacion

- Historias de usuario con criterios Gherkin en `docs/business/historias_usuario.md`.
- Contratos JSON en `docs/architecture/contratos/`.
- Metodos HTTP documentados en `docs/architecture/README.md`.

## Trazabilidad General

| Historia | Pantalla Figma | Contrato JSON |
|----------|----------------|---------------|
| HU-001 Registro y verificacion de usuario | Login / Registro | `docs/architecture/contratos/registro_usuario.json` |
| HU-002 Publicacion de viaje | Home / Publicar viaje | No requerido en esta iteracion de contratos |
| HU-003 Busqueda y solicitud de viaje | Busqueda de viajes | `docs/architecture/contratos/busqueda_viajes.json` |
| HU-004 Notificaciones | Home / Notificaciones | No requerido en esta iteracion de contratos |

## Historial de Pull Requests

| PR | Entregable |
|----|------------|
| https://github.com/DiegoRiv10/car-pooling/pull/1 | Tablero operativo y backlog inicial |
| https://github.com/DiegoRiv10/car-pooling/pull/2 | Historias de usuario refinadas |
| https://github.com/DiegoRiv10/car-pooling/pull/3 | Modelado JSON y metodos HTTP |

## Estado Final

El repositorio contiene la documentacion final del MVP sin codigo fuente de programacion, organizada por negocio, diseno y arquitectura conforme a los lineamientos de cierre y calidad.
