# Solución: Ejercicio 6 - Responsive Design

## Explicación de la solución

### 1. Viewport Meta Tag
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
**ESENCIAL** para que el navegador en móviles escale correctamente

### 2. Menú Hamburguesa Responsivo

**HTML:**
```html
<button class="menu-toggle" id="menuToggle">☰</button>
<nav class="nav" id="nav">...</nav>
```

**CSS (Desktop):**
```css
.menu-toggle {
  display: none;  /* Escondido en desktop */
}

.nav {
  display: flex;  /* Visible en desktop */
}
```

**CSS (Móvil, máx 768px):**
```css
.menu-toggle {
  display: block;  /* Visible en móvil */
}

.nav {
  display: none;  /* Escondido por defecto */
}

.nav.active {
  display: flex;  /* Visible cuando está activo */
}
```

### 3. Layout Responsive con Grid

**Desktop (3 columnas):**
```css
.container {
  grid-template-columns: 200px 1fr 250px;
}
```

**Tablets (1 columna con cambio de orden):**
```css
@media (max-width: 768px) {
  .container {
    grid-template-columns: 1fr;
  }
  
  .sidebar { order: 2; }
  .main { order: 1; }
  .ads-sidebar { order: 3; }
}
```

**Móviles (ajustes adicionales):**
```css
@media (max-width: 480px) {
  .container {
    padding: 0 10px;
  }
  
  .main h2 {
    font-size: 18px;  /* Reducir para caber en pantalla */
  }
}
```

### 4. Mobile-First vs Desktop-First

**Desktop-First (lo que hemos hecho):**
- Estilos principales para desktop
- Media queries que van restringiendo (max-width)

**Mobile-First (alternativa):**
- Estilos principales para móvil
- Media queries que van expandiendo (min-width)

### 5. Breakpoints comunes
```
Móvil:    < 480px
Tablet:   480px - 768px
Laptop:   769px - 1024px
Desktop:  > 1024px
```

### 6. Unidades Responsivas

| Unidad | Descripción | Ejemplo |
|--------|-------------|---------|
| `px` | Píxeles fijos | `font-size: 16px` |
| `%` | Porcentaje del padre | `width: 50%` |
| `em` | Relativo a tamaño de fuente actual | `margin: 2em` |
| `rem` | Relativo a tamaño de fuente raíz | `font-size: 1.5rem` |
| `vw` | Ancho del viewport | `width: 100vw` |
| `vh` | Alto del viewport | `height: 100vh` |

## JavaScript simple para el menú
```javascript
document.getElementById('menuToggle').addEventListener('click', function() {
  document.getElementById('nav').classList.toggle('active');
});
```

## Verificar Responsividad
- Abre DevTools (F12)
- Presiona Ctrl+Shift+M (o Cmd+Shift+M en Mac)
- Prueba diferentes tamaños de pantalla

## Buenas prácticas
✅ Siempre incluir viewport meta tag
✅ Usar unidades relativas cuando sea posible
✅ Probar en dispositivos reales
✅ Prioritizar contenido en móvil
✅ Usar mobile-first si es posible
