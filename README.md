# 🚗 Car-Pooling — Transporte Universitario

## Dashboard del Proyecto

| Campo | Detalle |
|-------|---------|
| **Proyecto** | Car-Pooling Universitario |
| **Equipo** | Diego Rivera · Sebastián Lugo · Diego Quintero |
| **Sesión actual** | Sesión 2 |
| **Estado** | 🟢 En progreso |
| **Tablero operativo** | [Jira - Car-Pooling](https://cesunbc-team-ztwxd7jm.atlassian.net/jira/software/projects/CPTU/list?jql=project+%3D+CPTU+ORDER+BY+cf%5B10019%5D+ASC&atlOrigin=eyJpIjoiMjE1MGY3OTVkNTlmNDllMjhmNzk3MjIwNDlhM2Q5NjAiLCJwIjoiaiJ9) |

---

## 👥 Equipo y Roles

| Integrante | Rol | Responsabilidad |
|------------|-----|-----------------|
| Diego Rivera | Scrum Master | Gestión del flujo de trabajo, revisión y aprobación de PRs, merge a main |
| Sebastián Lugo | Product Owner | Priorización del backlog, validación de entregas contra la visión del MVP |
| Diego Quintero | Development Lead | Arquitectura técnica, estructura de código y documentación de ingeniería |

---

## 🎯 Visión del MVP

### El Problema (Pain Point)
Los estudiantes universitarios enfrentan dificultades diarias para trasladarse a la universidad: el transporte público es ineficiente, costoso o inseguro, y muchos compañeros viajan solos en sus autos con asientos vacíos. No existe un canal confiable y organizado para coordinar viajes compartidos entre la comunidad estudiantil.

### La Propuesta de Valor
Una plataforma que conecta a estudiantes que se dirigen a la misma universidad, permitiéndoles compartir viajes de forma segura, económica y coordinada. Los conductores publican sus rutas y horarios, y los pasajeros solicitan unirse, reduciendo costos de transporte y la huella de carbono.

### El Alcance Crítico (MVP)
Las funciones mínimas sin las cuales el producto no existe:
1. **Registro y autenticación de usuarios** — Verificación con correo institucional.
2. **Publicación de viajes** — El conductor crea un viaje con origen, destino, horario y asientos disponibles.
3. **Búsqueda y solicitud de viaje** — El pasajero busca viajes disponibles y solicita unirse.
4. **Sistema de notificaciones** — Confirmación/rechazo de solicitudes y recordatorios de viaje.

### Métrica de Éxito
- Lograr al menos **20 viajes compartidos** coordinados a través de la plataforma durante el primer mes de prueba.
- Alcanzar una tasa de **80% de satisfacción** entre los usuarios que completen un viaje.

---

## 📁 Estructura del Repositorio

```
car-pooling/
├── management/          # Gestión estratégica del proyecto
│   ├── presupuesto.md   # Presupuesto inicial
│   ├── roi.md           # Cálculo de Retorno de Inversión
│   ├── backlog.csv      # Exportación del Backlog (Jira/Trello)
│   └── backlog-inicial.md # Backlog operativo de la Sesión 2
│
├── docs/                # Documentación de ingeniería
│   ├── historias-de-usuario.md
│   ├── diccionario-de-datos.md
│   ├── matriz-de-riesgos.md
│   └── entrega-sesion-2.md # Checklist y flujo de PR de la Sesión 2
│
├── prototypes/          # Activos de diseño y UX
│   ├── figma-link.md    # Enlace permanente a Figma
│   └── screenshots/     # Capturas del prototipo
│
└── README.md            # 📍 Este archivo (Dashboard)
```

---

## 🔄 Flujo de Trabajo

1. **Branching** — Cada entregable se trabaja en una rama separada (ej: `feat-session-1`).
2. **Pull Request** — Al terminar, se crea un PR hacia `main`.
3. **Code Review** — El Scrum Master (Diego Rivera) revisa y aprueba.
4. **Merge** — Integración final a la rama `main`.

> ⚠️ **Regla de Oro:** *"Todo debe estar en la rama main para que cuente como entregado y ser calificado."*

### Entregable Sesion 2

- [Backlog inicial](management/backlog-inicial.md)
- [Backlog en CSV para tablero](management/backlog.csv)
- [Guia de entrega y Pull Request](docs/entrega-sesion-2.md)

---

## 📅 Bitácora de Avance Semanal

| Sesión | Fecha | Entregable | Estado |
|--------|-------|------------|--------|
| 1 | — | Repo, estructura de carpetas, README con visión del MVP | ✅ Completado |
| 2 | — | Tablero operativo y backlog inicial con 12 tareas asignadas | ✅ Completado |
| 3 | — | Pendiente | ⬜ |
| 4 | — | Pendiente | ⬜ |

---

*Repositorio mantenido por el equipo Car-Pooling © 2025*
