# MangaCSS v2.0 🖊️📦 Blanco, Negro, Caos y Drama

**Librería 100% CSS+HTML con estilo manga** para cualquier web: landing pages, portfolios, e-commerce, blogs, o simplemente para darle un toque de viñeta a tus proyectos. Sin dependencias, sin JavaScript, sin complicaciones. Solo HTML y CSS puro con ese toque de tinta.

![MangaCSS]
<img width="1304" height="372" alt="Image" src="https://github.com/user-attachments/assets/bc911d3b-5a64-41ab-bd28-659ad385707a" />

🚀 **Características principales**

- **100% CSS + HTML** – Cero JavaScript, cero dependencias.
- **Estilo manga auténtico** – Viñetas, globos de diálogo, onomatopeyas, fondos de screentone, líneas de velocidad.
- **Totalmente responsive** – Grillas flexibles que se adaptan a móviles y tablets.
- **Componentes modernos** – Cards, botones, navbar, hero sections, badges, tooltips.
- **Filtros de imagen** – Efectos B&W, sepia, alto contraste, halftone, con hover a color.
- **Animaciones** – Shake, pulse, float, slam, ink reveal y más.
- **Fácil de personalizar** – Variables CSS para colores, bordes, sombras, tipografías.

📦 **Instalación**

Descarga directa
```bash
# Clona o descarga el archivo CSS
curl -O https://raw.githubusercontent.com/JZ-Dev0/MangaCSS/main/mangacss.css

```

CDN (si lo tienes alojado)
```html
<link rel="stylesheet" href="https://raw.githubusercontent.com/JZ-Dev0/MangaCSS/main/mangacss.css">
```

npm (próximamente)
```bash
npm install mangacss
```

Luego simplemente inclúyelo en tu HTML:
```html
<link rel="stylesheet" href="mangacss.css">
```

🎨 **Uso básico**

Estructura mínima para una página con estilo manga:
```html
<body>
  <div class="manga-page">
    <!-- Tus viñetas aquí -->
    <div class="panel-grid panel-grid-duo">
      <div class="panel">
        <img src="imagen.jpg" class="panel-img panel-img-bw">
        <div class="panel-inner">
          <div class="bubble-talk">¡Hola!</div>
        </div>
      </div>
      <div class="panel panel-dark">
        <span class="sfx-lg sfx-outline">POW!</span>
      </div>
    </div>
  </div>
</body>
```

📚 **Documentación completa**

## 1. Página manga (.manga-page)
Contenedor principal que simula una hoja de papel.
```html
<div class="manga-page"> ... </div>
<div class="manga-page-full"> ... </div> <!-- ancho completo -->
```

## 2. Paneles / Viñetas (.panel)

| Clase | Descripción |
|---|---|
| .panel | Viñeta base con borde negro |
| .panel-dark | Fondo negro, texto blanco |
| .panel-borderless | Sin bordes |
| .panel-double-border | Borde doble (con outline) |
| .panel-tilted-left | Rotación -1.5° |
| .panel-tilted-right | Rotación +1.5° |
| .panel-tilted-big | Rotación -3° |
| .panel-shadow / .panel-shadow-lg | Sombra manga |
| .panel-rounded / .panel-rounded-lg / .panel-pill | Bordes redondeados |
| .panel-accent | Borde de color acento |
| .panel-hover / .panel-hover-grow / .panel-hover-tilt | Efectos hover |

## 3. Grillas de viñetas (.panel-grid-*)
```html
<div class="panel-grid panel-grid-duo"> ... </div>
```
Clases disponibles: `solo`, `duo`, `trio`, `quad`, `main-side`, `side-main`, `hero-duo`, `duo-hero`, `asymmetric`, `golden`, `golden-reverse`, `magazine`, `mosaic`, `cascade`, `auto`.

## 4. Imágenes manga (.panel-img-*)
| Clase | Efecto |
|---|---|
| .panel-img-bw | B&N con hover a color |
| .panel-img-manga | Alto contraste |
| .panel-img-ink | Multiplicar (tinta) |
| .panel-img-sepia | Sepia con hover a color |
| .panel-img-poster | B&N extremo |
| .panel-img-halftone | Efecto medio tono |

**Overlays**:
- `.panel-img-overlay-bottom` – Gradiente oscuro desde abajo
- `.panel-img-overlay-top` – Gradiente oscuro desde arriba
- `.panel-img-overlay-full` – Capa semitransparente

## 5. Fondos especiales (.bg-*)
| Clase | Descripción |
|---|---|
| .bg-halftone | Puntos (medio tono) |
| .bg-halftone-dark | Puntos sobre negro |
| .bg-speed-h / .bg-speed-v | Líneas de velocidad |
| .bg-radial-lines | Líneas radiales |
| .bg-crosshatch | Rayado cruzado |
| .bg-noise | Granulado |
| .bg-stripe-h / .bg-stripe-diagonal | Rayas |
| .bg-tone-light/mid/dark | Tonos planos |

## 6. Globos de diálogo (.bubble-*)
```html
<div class="bubble-talk">¡Hola!</div>
<div class="bubble-think">...mmm...</div>
<div class="bubble-shout">¡¡NO!!</div>
<div class="bubble-explosive">¡¡ATAQUE!!</div>
<div class="bubble-dark">Soy el malo</div>
<div class="bubble-whisper">secreto</div>
<div class="bubble-accent">¡OFERTA!</div>
```
Direcciones: `.bubble-right`, `.bubble-top`.

## 7. Onomatopeyas (.sfx-*)
| Clase | Tamaño / Estilo |
|---|---|
| .sfx-sm / .md / .lg / .xl / .mega | Tamaños |
| .sfx-outline | Borde negro, relleno blanco |
| .sfx-solid | Negro sólido |
| .sfx-white | Blanco con borde |
| .sfx-accent | Color acento con borde |
| .sfx-slant-left/right/big | Rotación |
| .sfx-skew | Deformación |

## 8. Botones (.manga-btn-*)
```html
<a class="manga-btn">Normal</a>
<a class="manga-btn manga-btn-dark">Dark</a>
<a class="manga-btn manga-btn-accent">¡Comprar!</a>
<a class="manga-btn manga-btn-outline">Outline</a>
<a class="manga-btn manga-btn-pill manga-btn-lg">Grande</a>
```

## 9. Cards (.manga-card)
```html
<div class="manga-card">
  <img src="..." class="manga-card-img">
  <div class="manga-card-body">
    <div class="manga-card-title">Título</div>
    <div class="manga-card-text">Descripción</div>
    <span class="manga-card-price">$29.99</span>
    <span class="manga-card-price-old">$49.99</span>
  </div>
  <div class="manga-card-footer"> ... </div>
</div>
```

## 10. Navbar (.manga-nav)
```html
<nav class="manga-nav">
  <a class="manga-nav-brand">MANGA<span>CSS</span></a>
  <ul class="manga-nav-links">
    <li><a href="#">Inicio</a></li>
    <li><a href="#">Productos</a></li>
  </ul>
</nav>
```

## 11. Badges y Tags
```html
<span class="manga-badge">Default</span>
<span class="manga-badge manga-badge-accent">Oferta</span>
<span class="manga-tag">HTML</span>
<span class="manga-tag manga-tag-filled">CSS</span>
```

## 12. Hero Section (.manga-hero)
```html
<div class="manga-hero">
  <img src="bg.jpg" class="manga-hero-bg">
  <div class="manga-hero-overlay manga-hero-overlay-halftone"></div>
  <div class="manga-hero-content">
    <h1 class="manga-title manga-title-white">¡BIENVENIDO!</h1>
    <a class="manga-btn manga-btn-accent">Explorar</a>
  </div>
</div>
```

## 13. Tipografía
Clases: `.manga-title`, `.manga-title-sm`, `.manga-title-xl`, `.manga-title-outline`, `.manga-title-accent`, `.manga-body`, `.manga-body-sm`, `.manga-body-lg`, `.manga-subtitle`, `.manga-caption`, `.manga-text-vertical`

## 14. Animaciones
| Clase | Descripción |
|---|---|
| .anim-shake / .anim-shake-hover | Sacudida |
| .anim-pulse | Latido |
| .anim-float | Flotación suave |
| .anim-slam | Impacto |
| .anim-slide-up / .anim-slide-left | Deslizamiento |
| .anim-fade-in | Aparición |
| .anim-ink-reveal | Revelado tipo tinta |
| .anim-delay-1 al 5 | Retardos |

## 15. Utilidades
- Espaciado: `.manga-p-sm/md/lg/xl`, `.manga-gap-sm/md/lg`
- Flex: `.manga-flex`, `.manga-flex-center`, `.manga-flex-col`
- Texto: `.manga-text-left/center/right`
- Ancho: `.manga-w-full`, `.manga-w-half`, `.manga-mw-sm/md/lg/xl`
- Rotaciones: `.rotate-1`, `.rotate--2`, etc.
- Z-index: `.z-top`, `.z-high`, `.z-low`

🌟 **Ejemplo completo: landing page e-commerce**
```html
<nav class="manga-nav">
  <a class="manga-nav-brand">MANGA<span style="opacity:.4">SHOP</span></a>
  <ul class="manga-nav-links">
    <li><a href="#">Tienda</a></li>
    <li><a href="#" class="manga-btn manga-btn-sm manga-btn-accent">🛒 Carrito</a></li>
  </ul>
</nav>

<div class="manga-hero">
  <img src="hero.jpg" class="manga-hero-bg">
  <div class="manga-hero-overlay manga-hero-overlay-halftone"></div>
  <div class="manga-hero-content">
    <div class="manga-title manga-title-white">¡MEGA OFERTA!</div>
    <a class="manga-btn manga-btn-accent">Ver Ofertas</a>
  </div>
</div>

<div class="panel-grid panel-grid-trio">
  <div class="manga-card">
    <img src="producto.jpg" class="manga-card-img">
    <div class="manga-card-body">
      <div class="manga-card-title">Camiseta Manga</div>
      <div class="manga-card-price">$21.00</div>
    </div>
    <div class="manga-card-footer">
      <a class="manga-btn manga-btn-sm manga-btn-accent">Comprar</a>
    </div>
  </div>
  <!-- más cards... -->
</div>
```

⚙️ **Personalización**

Todas las variables CSS están en `:root`. Puedes sobrescribirlas fácilmente:
```css
:root {
  --manga-black: #0a0a0a;
  --manga-white: #faf8f2;
  --manga-accent: #ff3d3d;
  --border-thick: 4px;
  --manga-shadow: 4px 4px 0 var(--manga-black);
  --font-impact: 'Bangers', cursive; /* ... */
}
```

📱 **Responsive**

La librería incluye media queries para móviles y tablets. Las grillas se apilan automáticamente. Clase auxiliar: `.hide-mobile` para ocultar elementos en pantallas pequeñas.

📄 **Licencia**

**MIT** – Haz lo que quieras, pero si la usas para algo épico, manda un saludo.

🖊️ 🤝 **Contribuciones**

¿Encontraste un bug? ¿Quieres añadir más estilos manga? Abre un issue o envía un pull request. Toda ayuda es bienvenida.

🙏 **Créditos**

Creada con amor, tinta y mucho café por **JZ DEV**.
Tipografías: Google Fonts (Bangers, Comic Neue, Permanent Marker, Special Elite, Oswald, Inter).

**MangaCSS v2.0 – Blanco, Negro, Caos y Drama. 「漫画」**
