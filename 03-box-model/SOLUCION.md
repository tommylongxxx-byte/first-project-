# Solución: Ejercicio 3 - Box Model

## Explicación de la solución

### El Box Model en práctica
Cada elemento tiene 4 capas:
1. **Margin** (20px) - espacio externo
2. **Border** (3px) - borde visible
3. **Padding** (20px) - espacio interno
4. **Content** - el texto y elementos dentro

### Cajas específicas

**Caja 1**:
- Margin: 10px arriba, 20px derecha, 30px abajo, 40px izquierda (clockwise)
- Border rojo sólido de 3px
- Background rojo claro

**Caja 2**:
- Margin simétrico: 20px arriba/abajo, 0 izquierda/derecha
- Border dashed (punteado) verde
- Padding diferente horizontalmente

**Caja 3**:
- `box-sizing: border-box` - el width incluye padding y border
- Sin esto, width + padding + border = ancho total mayor
- Width definido en 300px

**Caja Centrada**:
- `margin: 40px auto;` - centra horizontalmente
- Es el método clásico para centrar bloques
- Media query: se adapta a pantallas pequeñas

## Conceptos importantes
- Margin es transparente, padding tiene el color de fondo
- `box-sizing: border-box` es muy útil para cálculos precisos
- `margin: 0 auto;` centra elementos block
- Usa DevTools (F12) para inspeccionar el box model

## Practica
- Intenta cambiar los valores de margin y padding
- Prueba diferentes border-styles: solid, dashed, dotted, double
- Experimenta con border-radius para esquinas redondeadas
