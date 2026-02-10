# Solución: Ejercicio 5 - CSS Grid

## Explicación de la solución

### 1. Grid Simple 3x3
```css
.grid-container-simple {
  display: grid;
  grid-template-columns: repeat(3, 1fr);  /* 3 columnas iguales */
  gap: 10px;                               /* Espacio entre items */
}
```
- `repeat(3, 1fr)` crea 3 columnas de igual tamaño
- `1fr` = 1 fracción (divide el espacio disponible)
- `gap` es similar a flexbox

### 2. Layout de Página (Header, Nav, Main, Sidebar, Footer)
```css
.grid-container-page {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;    /* 3 columnas */
  grid-template-rows: auto auto auto;    /* 3 filas */
  gap: 15px;
}

.header {
  grid-column: 1 / -1;  /* De columna 1 a la última (-1) */
}

.nav {
  grid-column: 1;
  grid-row: 2 / 4;      /* De fila 2 a 4 */
}

.main {
  grid-column: 2;
  grid-row: 2 / 4;
}

.sidebar {
  grid-column: 3;
  grid-row: 2 / 4;
}

.footer {
  grid-column: 1 / -1;
}
```

### 3. Responsivo con Media Queries
- **Desktop (3 columnas)**: grid-template-columns: repeat(3, 1fr)
- **Tablet (2 columnas)**: grid-template-columns: repeat(2, 1fr)
- **Móvil (1 columna)**: grid-template-columns: 1fr

## Diferencia entre Flexbox y Grid

| Flexbox | Grid |
|---------|------|
| 1 dimensión (fila o columna) | 2 dimensiones (filas y columnas) |
| Perfecto para navegaciones | Perfecto para layouts de página |
| Orden flexible | Posicionamiento explícito |
| `justify-content`, `align-items` | `grid-column`, `grid-row` |

## Propiedades Grid importantes
- `grid-template-columns` - define el ancho de columnas
- `grid-template-rows` - define el alto de filas
- `grid-column: inicio / fin` - posiciona horizontalmente
- `grid-row: inicio / fin` - posiciona verticalmente
- `gap` - espaciado entre elementos
- `auto-fit`, `auto-fill` - responsivo automático

## Práctica adicional
- Usa `grid-template-areas` para un layout nombrado
- Experimenta con `minmax(100px, 1fr)`
- Prueba `auto-fit` y `auto-fill`
