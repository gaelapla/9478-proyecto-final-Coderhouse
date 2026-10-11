# Skincare Pro

Sitio web estático de 5 páginas para **Skincare Pro**, un emprendimiento de cuidado de la piel de Buenos Aires. Proyecto final del curso de Desarrollo Web de Coderhouse.

**Sitio publicado:** https://skincare-pro-gaela.netlify.app

## Páginas

| Página | Archivo |
|---|---|
| Inicio | `index.html` |
| Productos | `pages/productos.html` |
| Sobre nosotros | `pages/sobre-nosotros.html` |
| Preguntas frecuentes | `pages/preguntas-frecuentes.html` |
| Contacto | `pages/contacto.html` |

## Tecnologías

- **HTML5 semántico:** `nav`, `main`, `section`, `article`, `footer`.
- **SCSS** con variables, anidamiento, mixins con parámetros, `@extend` con placeholders y parciales organizados por carpetas. `main.scss` solo contiene los `@use`.
- **Bootstrap 5.3.3** (CDN) para el menú de navegación responsive y el carrusel, personalizado desde SCSS.
- **AOS 2.3.1** (CDN) para las animaciones al hacer scroll.
- **Tabler Icons** para los íconos.
- **Google Fonts:** Poppins y Lato.

## Animaciones

- **Nativas (CSS):** transiciones al pasar el mouse sobre las tarjetas (mixin `hover-elevar`) y `@keyframes aparecer-tarjeta` en las tarjetas de productos destacados.
- **Con librería:** AOS (`fade-right`, `fade-left`) en la sección de medios de pago.

## Diseño responsive

Se probó en tres anchos, sin scroll horizontal:

- **Celular:** 375 px (mixin `mobile-chico`, hasta 480 px)
- **Tablet:** 768 px (mixin `tablet`)
- **Compu:** 1280 px (mixin `desktop`, desde 1024 px)

## SEO y accesibilidad

- Cada página tiene su propio `title`, `meta description` y `meta keywords`.
- Todas las imágenes tienen texto alternativo (`alt`).
- Los colores de acento oscuros (`$color-acento-oscuro`, `$color-verde-oscuro`) se usan en botones y textos para mejorar el contraste.

## Estructura del proyecto

```
├── index.html
├── pages/
│   ├── productos.html
│   ├── sobre-nosotros.html
│   ├── preguntas-frecuentes.html
│   └── contacto.html
├── scss/
│   ├── main.scss
│   ├── base/
│   ├── components/
│   ├── layout/
│   └── utilities/        (variables y mixins)
├── styles/
│   └── main.css          (CSS compilado)
└── assets/               (imágenes)
```

## Cómo compilar los estilos

Los estilos se escriben en `scss/` y se compilan a `styles/main.css`. Con la extensión **Live Sass Compiler** de VS Code, se activa con el botón **Watch Sass**. También se puede compilar con:

```
npx sass scss/main.scss styles/main.css
```

## Autora

Gaela Carreira, Buenos Aires.