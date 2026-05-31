# Entrega Sesion 3 - Refinamiento y Reestructura de Historias

## Objetivo de la sesion

Redactar las 4 historias de usuario principales del MVP con formato oficial, crear o reflejar esas historias en Jira y vincular las tareas de la Sesion 2 como subtareas.

## Checklist de entrega

- [x] Redactar 4 historias principales del MVP.
- [x] Incluir formato oficial: Como / quiero / para.
- [x] Agregar criterios de aceptacion por historia.
- [x] Vincular las tareas de la Sesion 2 como subtareas sugeridas.
- [x] Actualizar `docs/historias_de_usuario.md`.
- [x] Preparar CSV de apoyo para crear historias y subtareas en Jira.
- [ ] Crear las historias en Jira como issues tipo `Story`.
- [ ] Vincular las tareas de la Sesion 2 como `Sub-task` o tareas relacionadas.
- [ ] Integrar los cambios a `main` mediante Pull Request.

## Archivos actualizados

- `docs/historias_de_usuario.md`
- `docs/historias-de-usuario.md`
- `management/jira-historias-sesion-3.csv`

## Historias principales

| ID | Historia | Prioridad |
|----|----------|-----------|
| HU-001 | Registro y verificacion de usuario | Alta |
| HU-002 | Publicacion de viaje | Alta |
| HU-003 | Busqueda y solicitud de viaje | Alta |
| HU-004 | Notificaciones de solicitudes y recordatorios | Media |

## Flujo de Jira recomendado

1. Crear las historias HU-001 a HU-004 como issues tipo `Story`.
2. Crear las tareas CP correspondientes debajo de cada historia como `Sub-task`.
3. Revisar que cada historia tenga responsable y prioridad.
4. Confirmar que el tablero muestre la reestructura del backlog.

## Flujo de GitHub recomendado

```bash
git switch -c session-3-historias-usuario
git add README.md docs/historias_de_usuario.md docs/historias-de-usuario.md docs/entrega-sesion-3.md management/jira-historias-sesion-3.csv
git commit -m "docs(session-3): refinar historias de usuario"
git push -u origin session-3-historias-usuario
```

Despues de subir la rama:

1. Abrir Pull Request hacia `main`.
2. Revisar que `docs/historias_de_usuario.md` contenga las 4 historias.
3. Hacer merge del Pull Request.
