# Frontend Mentor - Blog Preview Card Solution

Esta es mi solución al [reto del componente de tarjeta de vista previa de blog en Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS).

## Información del proyecto

### El reto
Los usuarios deben ser capaces de:
- Ver los estados de hover y focus para todos los elementos interactivos de la página (como el título del artículo).
- Ver el diseño óptimo para el componente dependiendo del tamaño de pantalla de su dispositivo (Responsivo).

### Captura de pantalla
![Diseño Final](./images/screenshot.png)

### Enlaces
- URL del Repositorio: [https://github.com/EdgardoGuerrero/frontend-mentor-challenges](https://github.com/EdgardoGuerrero/frontend-mentor-challenges)
- URL del Sitio Web Vivo: [https://edgardoguerrero.github.io/frontend-mentor-challenges/blog-preview-card-main/](https://edgardoguerrero.github.io/frontend-mentor-challenges/blog-preview-card-main/)

## Mi proceso

### Tecnologías utilizadas
- Marcado HTML5 semántico (`<article>`, `<main>`, `<footer>`)
- Propiedades personalizadas de CSS (Variables)
- Flexbox (Diseño de caja flexible)
- Metodología de nomenclatura basada en bloques para las clases (`.article-card`, `.article-title`, etc.)
- Enfoque Mobile-first

### Qué aprendí
En este reto profundicé en la semántica avanzada de HTML y en buenas prácticas de seguridad web:

1. **Uso correcto de `<article>`:** Aprendí que para componentes que representan bloques de contenido independientes y reutilizables (como una tarjeta de blog o un producto), la etiqueta semántica ideal es `<article>` en lugar de un `<div>` genérico. Esto encaja perfectamente con la arquitectura de clases `.article-card` y mejora la accesibilidad.
2. **Fechas accesibles:** En lugar de renderizar la fecha en un `span` común, utilicé la etiqueta `<time>` junto con el atributo `datetime` para que los lectores de pantalla y los motores de búsqueda (SEO) puedan interpretar datos temporales de forma eficiente:
```html
   <time datetime="2023-12-21" class="article-publication-date">Published 21 Dec 2023</time>