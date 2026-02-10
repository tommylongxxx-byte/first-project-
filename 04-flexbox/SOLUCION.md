# Solución: Ejercicio 4 - Flexbox

## Explicación de la solución

### 1. Barra de Navegación
```css
.navbar {
  display: flex;
  justify-content: space-around;  /* Distribuye elementos uniformemente */
  align-items: center;            /* Centra verticalmente */
  background-color: #333;
  padding: 15px 0;
}
```
- `flex` activa Flexbox
- `justify-content: space-around` distribuye los enlaces uniformemente
- `align-items: center` los centra verticalmente

### 2. Tarjetas con Flexbox
```css
.cards {
  display: flex;
  flex-wrap: wrap;                /* Permite que las tarjetas se envuelvan */
  gap: 20px;                       /* Espacio entre tarjetas */
  justify-content: center;
}

.card {
  flex: 0 0 calc(33.333% - 20px); /* 3 columnas */
}
```
- `flex-wrap: wrap` permite que las tarjetas vayan a la siguiente línea
- `calc(33.333% - 20px)` para que 3 tarjetas quepan con el gap
- `gap` es más limpio que margin

### 3. Layout de Dos Columnas
```css
.main-layout {
  display: flex;
  min-height: 400px;
}

.sidebar {
  flex: 0 0 25%;  /* No crece, no se encoge, 25% de ancho */
}

.content {
  flex: 1;        /* Ocupa el espacio restante */
}
```

## Responsive
- En pantallas medianas: tarjetas de 2 columnas
- En pantallas pequeñas: tarjetas de 1 columna
- El layout se convierte en vertical (`flex-direction: column`)

## Propiedades flex resumidas
- `flex: 1` = crece, se encoge naturalmente
- `flex: 0 0 25%` = tamaño fijo, no crece ni se encoge
- `gap` = espaciado automático entre items (más limpio que margin)

## Práctica adicional
- Prueba `justify-content` con valores: flex-start, flex-end, center, space-between, space-evenly
- Prueba `align-items` con valores: flex-start, flex-end, center, stretch
- Experimenta con `flex-direction: column`
