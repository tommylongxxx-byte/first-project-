# Ejercicio 6: Responsive Design

## Objetivos
- Aprender Mobile-First
- Dominar Media Queries
- Crear diseños adaptables

## Conceptos clave

### Viewport Meta Tag
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
Obligatorio para sitios responsive

### Media Queries
```css
@media (max-width: 768px) {
  /* Estilos para pantallas pequeñas */
}
```

### Breakpoints comunes
- **Mobile**: < 480px
- **Tablets**: 481px - 768px
- **Laptops**: 769px - 1024px
- **Desktop**: > 1024px

### Unidades responsivas
- `%` - porcentaje del padre
- `em` - relativo al tamaño de fuente actual
- `rem` - relativo al tamaño de fuente raíz
- `vw` - ancho de la ventana (viewport width)
- `vh` - alto de la ventana

## Tareas

### Tarea 1: Crea una navegación responsive
1. En desktop: menú horizontal
2. En móvil: menú hamburguesa (necesita JS después)
3. Usa `display: none/block` para esconder/mostrar elementos

### Tarea 2: Crear layout adaptable
1. Desktop: 3 columnas (sidebar, main, ads)
2. Tablet: 2 columnas (sidebar + main, ads abajo)
3. Móvil: 1 columna (todo apilado)

### Tarea 3: Tipografía responsiva
1. Tamaño de fuente diferente según pantalla
2. Padding/margin que se ajusten
3. Líneas de lectura óptimas (60-80 caracteres)

---

Ver `SOLUCION.md` cuando termines.
