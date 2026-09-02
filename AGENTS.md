# AGENTS.md

## Ejecución
- Sin build: abrir `index.html` directamente o `npx serve .`
- Canvas fijo 800×600 (hardcoded en `game.js`)

## Estructura
- Todo el juego en un solo archivo: `game.js` (~420 líneas)
- Sin dependencias, sin bundler, sin módulos
- `index.html` solo carga CSS inline + `game.js`

## Herramientas
- No hay tests, linter, typecheck, ni CI
- No hay `package.json`
