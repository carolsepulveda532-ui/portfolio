# Portafolio — Carol Yined Sepúlveda Flórez

Sitio estático (HTML5 + CSS3 + JavaScript + Bootstrap 5 + AOS + Font Awesome), estilo *Dark Minimalist*.

## Cómo verlo
Abre `index.html` en el navegador, o sirve la carpeta con cualquier servidor estático:

```bash
npx serve .
# o
python -m http.server 8000
```

## Qué falta personalizar (marcado con placeholders)

1. **Foto de perfil** — en `index.html`, dentro de `.portrait-photo`, reemplaza el bloque `<span class="portrait-initials">CS</span>` por:
   ```html
   <img src="img/carol.jpg" alt="Carol Yined Sepúlveda Flórez">
   ```
   y coloca tu foto en `img/carol.jpg`.

2. **CV en PDF** — coloca tu CV real en `cv/CV-Carol-Sepulveda.pdf` (los botones "Descargar CV" ya apuntan ahí).

3. **Correo, WhatsApp y enlaces de proyectos** — en la sección `#contacto`, reemplaza el correo de ejemplo y el enlace de WhatsApp por los tuyos. Actualiza los enlaces `github.com/carolsepulveda532-ui` de cada proyecto por el repositorio específico de cada uno, y agrega el link de demo si tienes uno desplegado (Netlify, Vercel, GitHub Pages).

4. **Formulario de contacto** — actualmente el formulario solo valida y muestra un mensaje de confirmación en el navegador (no envía correos reales). Para que funcione de verdad, conéctalo a un servicio como Formspree, EmailJS o un backend propio.

5. **Proyectos** — hay 4 proyectos de ejemplo ya redactados con tu información real (Sistema Bancario, Rutas & Destinos, TrendyShop, NASA APOD Explorer). Actualiza imágenes reales (`.project-card__media`) cuando tengas capturas de pantalla, y agrega más proyectos copiando el bloque `<article class="project-card">`.

## Estructura

```
/portfolio
  index.html
  /css
    style.css
  /js
    script.js
  /img        ← fotos y capturas de pantalla
  /assets     ← otros recursos
  /cv         ← CV en PDF
```

## Notas de diseño

- Paleta: negro profundo `#0B0B0B`, gris oscuro `#181818`, blanco hueso `#F5F5F2`, dorado `#C9A86A`, gris claro `#9E9E9E`.
- Tipografías: Playfair Display (títulos) + Inter (cuerpo).
- El elemento distintivo del sitio es el **hilo dorado** (línea SVG que se dibuja en el hero) y el marco floral inspirado en el moodboard, que reaparece de forma sutil junto al retrato — un guiño elegante en lugar de una foto de stock genérica.
- Navbar transparente al inicio, con efecto *glass* sutil al hacer scroll.
- Accesible: foco visible en todos los elementos interactivos, `prefers-reduced-motion` respetado, formulario con validación nativa.
- Responsive: probado en punto de quiebre móvil, tablet y escritorio (Bootstrap grid + media queries propias).
