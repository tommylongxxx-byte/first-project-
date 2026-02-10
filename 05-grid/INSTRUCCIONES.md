# Ejercicio 5: CSS Grid

## Objetivos
- Dominar el layout con CSS Grid
- Entender grid-template-columns y filas
- Crear layouts complejos y bidimensionales

## Conceptos clave

### Propiedades del contenedor grid
- `display: grid;` - activa CSS Grid
- `grid-template-columns: 1fr 2fr 1fr;` - define ancho de columnas
- `grid-template-rows: 100px 200px;` - define alto de filas
- `gap: 20px;` - espacio entre elementos
- `grid-auto-flow: dense;` - como se llenan las celdas

### Unidades en Grid
- `fr` (fracción) - divide el espacio disponible
- `repeat()` - repite un patrón
- `minmax()` - tamaño mínimo y máximo

### Posicionamiento en Grid
- `grid-column: 1 / 3;` - ocupa de columna 1 a 3
- `grid-row: 1 / 2;` - ocupa de fila 1 a 2

## Tareas

### Tarea 1: Crea un grid simple 3x3
1. Contenedor grid con 3 columnas igual de anchas
2. 9 items (cajas de colores)
3. Gap de 10px

### Tarea 2: Crea un layout de página (header, nav, main, sidebar, footer)
1. Header ocupa todo el ancho (columna 1 a 4)
2. Nav en columna 1 (2 filas)
3. Main en columnas 2-3 (2 filas)
4. Sidebar en columna 4 (2 filas)
5. Footer ocupa todo el ancho (columna 1 a 4)

### Tarea 3: Crea un grid responsivo
1. 3 columnas en desktop
2. 2 columnas en tablets
3. 1 columna en móviles

---

Ver `SOLUCION.md` cuando termines.
