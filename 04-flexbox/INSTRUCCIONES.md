# Ejercicio 4: Flexbox

## Objetivos
- Dominar el modelo de layout Flexbox
- Entender dirección, alineación y distribución de elementos
- Crear layouts flexibles y responsivos

## Conceptos clave

### Propiedades del contenedor flex
- `display: flex;` - activa flexbox
- `flex-direction: row | column;` - dirección (horizontal o vertical)
- `justify-content: flex-start | center | space-between | space-around;` - alineación en el eje principal
- `align-items: flex-start | center | stretch;` - alineación en el eje transversal
- `flex-wrap: wrap | nowrap;` - permite que los items se envuelvan

### Propiedades de los items flex
- `flex: 1;` - crece para ocupar espacio disponible
- `flex-grow: 1;` - define cómo crece
- `flex-shrink: 1;` - define cómo se encoge
- `flex-basis: 200px;` - tamaño base del item

## Tareas

### Tarea 1: Crea una barra de navegación con Flexbox
1. Crea un contenedor `<nav>` con `display: flex;`
2. Agrega 5 enlaces `<a>` dentro
3. Usa `justify-content: space-around;` para distribuirlos
4. Estiliza los enlaces

### Tarea 2: Crea un layout de tarjetas
1. Crea un contenedor con `display: flex;` y `flex-wrap: wrap;`
2. Agrega 6 tarjetas (div)
3. Cada tarjeta ocupa 1/3 del ancho en escritorio
4. Usa `align-items: center;` para centrar el contenido

### Tarea 3: Crea un layout de dos columnas
1. Contenedor principal con `flex-direction: row;`
2. Sidebar izquierdo (`flex: 0 0 25%;`)
3. Contenido principal (`flex: 1;`)

---

Ver `SOLUCION.md` cuando termines.
