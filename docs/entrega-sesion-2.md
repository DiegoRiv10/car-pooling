# Entrega Sesion 2 - Tablero Operativo y Backlog Inicial

## Objetivo de la sesion

Crear un tablero operativo para el equipo, desglosar el MVP en tareas atomicas y dejar evidencia del flujo de trabajo mediante Pull Request.

## Checklist de entrega

- [ ] Crear tablero en Jira o Trello.
- [ ] Configurar columnas minimas: `Por hacer`, `En progreso`, `En revision`, `Hecho`.
- [ ] Crear al menos 10 tarjetas del backlog inicial.
- [ ] Asignar responsable a cada tarjeta.
- [ ] Compartir el tablero con enlace publico o visible para el profesor.
- [ ] Pegar el enlace del tablero en `README.md` y `management/backlog-inicial.md`.
- [ ] Subir cambios a una rama de trabajo.
- [ ] Abrir Pull Request hacia `main`.
- [ ] Realizar merge del Pull Request.

## Tarjetas sugeridas para el tablero

Las tarjetas estan documentadas en:

- `management/backlog-inicial.md`
- `management/backlog.csv`

El archivo `management/backlog.csv` puede copiarse como base para importar o crear tarjetas en el tablero.

## Flujo de GitHub recomendado

```bash
git switch -c session-2-tablero-backlog
git add README.md docs/entrega-sesion-2.md management/backlog.csv management/backlog-inicial.md
git commit -m "feat(session-2): agregar tablero operativo y backlog inicial"
git push -u origin session-2-tablero-backlog
```

Despues de subir la rama:

1. Abrir el repositorio en GitHub.
2. Crear un Pull Request desde `session-2-tablero-backlog` hacia `main`.
3. Revisar que el README muestre el link publico del tablero.
4. Hacer merge del Pull Request.

## Evidencia esperada

- README con link del tablero.
- Tablero con minimo 10 tareas y responsables.
- Pull Request creado y mergeado hacia `main`.
