# Solución: Ejercicio 7 - Portafolio Personal

## Resumen de la solución

Este es un portafolio web completo que integra todos los conceptos aprendidos:

### ✅ Características implementadas

1. **HTML Semántico**
   - `<header>` con navegación
   - `<section>` para cada área (about, skills, projects, contact)
   - `<article>` para tarjetas de proyectos
   - `<footer>` apropiado
   - Estructura jerárquica clara

2. **CSS Avanzado**
   - Variables CSS (--primary-color, etc.)
   - Gradientes lineales en hero
   - Transiciones suaves en hover
   - Sombras y profundidad
   - Grid y Flexbox

3. **Responsive Design**
   - Mobile-first en algunas secciones
   - Breakpoints en 768px y 480px
   - Menú hamburguesa en móvil
   - Layout adaptable

4. **Interactividad (JS mínimo)**
   ```javascript
   // Menú hamburguesa
   document.getElementById('menuToggle').addEventListener('click', function() {
     document.getElementById('nav').classList.toggle('active');
   });
   ```

5. **Buenas prácticas de UX**
   - `scroll-behavior: smooth` para transiciones suaves
   - Efectos hover en botones
   - Formulario accesible
   - Contraste de colores adecuado

---

## Estructura de carpetas

```
07-portafolio/
├── index.html
├── style.css
└── assets/  (opcional para imágenes)
    ├── profile.jpg
    └── project-1.jpg
```

---

## Paleta de colores utilizada

| Variable | Color | Uso |
|----------|-------|-----|
| `--primary-color` | #3498db (Azul) | Enlaces, botones principales |
| `--secondary-color` | #2c3e50 (Gris oscuro) | Header, títulos |
| `--accent-color` | #e74c3c (Rojo) | CTA button, hover effects |
| `--light-bg` | #ecf0f1 (Gris claro) | Fondos alternos |

---

## Puntos clave de la solución

### 1. Variables CSS
```css
:root {
  --primary-color: #3498db;
  --secondary-color: #2c3e50;
  /* ... */
}
```
**Beneficio:** Cambiar colores en un lugar en lugar de todo el documento

### 2. Sticky Header
```css
.header {
  position: sticky;
  top: 0;
  z-index: 100;
}
```
**Beneficio:** Navegación siempre visible

### 3. Menú Responsivo
```html
<button class="menu-toggle" id="menuToggle">☰</button>
```
**Oculto en desktop, visible en móvil**

### 4. Cards con hover
```css
.project-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 25px rgba(0,0,0,0.15);
}
```
**Efecto de profundidad al pasar el mouse**

### 5. Formulario accesible
```html
<label for="name">Nombre</label>
<input type="text" id="name" name="name" required>
```
**Labels vinculados con for/id**

---

## Mejoras que podrías hacer

### Nivel 1 (Fácil)
- Cambiar colores de la paleta
- Agregar más proyectos
- Modificar texto personal
- Añadir imagen de perfil

### Nivel 2 (Intermedio)
- Agregar animaciones CSS
- Integrar Font Awesome para iconos
- Agregar Google Fonts
- Implementar dark mode

### Nivel 3 (Avanzado)
- Conectar formulario a backend (Flask/Node)
- Agregar JavaScript para interactividad
- Implementar animaciones AOS (Animate On Scroll)
- Optimizar SEO

---

## Validación de la solución

**Checklist:**
- ✅ Funciona en desktop, tablet y móvil
- ✅ Navegación funciona bien
- ✅ Formulario tiene validación HTML5
- ✅ Colores son coherentes
- ✅ Tipografía es legible
- ✅ Sin frameworks CSS (CSS puro)
- ✅ Código limpio y organizado

---

## Próximos pasos

Después de dominar este proyecto, puedes:
1. Agregar JavaScript interactivo
2. Crear una versión con Flask/Node
3. Publicar en GitHub Pages o Netlify
4. Mejorar el SEO
5. Agregar más secciones (blog, testimonios, etc.)

¡Este portafolio es el inicio de tu presencia online como desarrollador!
