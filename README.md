# TechLab Store - Pre-Entrega Front-End JS

**Curso:** Front-End JS  
**Institución:** Talento Tech (Agencia de Habilidades para el Futuro - Buenos Aires Ciudad)  
**Estudiante:** Gonzalo Orellana  
**Instancia:** Pre-Entrega de Proyecto (Clases 01 a 07 - HTML5 & CSS3)  
**Demo en Vivo (GitHub Pages):** [https://gonzaloorellana.github.io/proyecto-final-ecommerce-Gonzalo-Orellana/](https://gonzaloorellana.github.io/proyecto-final-ecommerce-Gonzalo-Orellana/)

---

## 📌 Propósito y Arquitectura del Sitio

TechLab Store es una plataforma web desarrollada como e-commerce y catálogo de periféricos y accesorios informáticos orientados a desarrolladores y estudiantes de programación.

El proyecto está diseñado bajo una arquitectura **multi-página** (no landing page de scroll único), cumpliendo estrictamente con la consigna de cursada:
- **`index.html`**: Página principal con hero, vitrina de categorías, grandes descuentos, novedades, newsletter y testimonios.
- **`pages/productos.html`**: Catálogo completo de productos con sistema de filtrado nativo por categorías (100% HTML5 y CSS3 puro con Flexbox).
- **`pages/contacto.html`**: Página dedicada con formulario de contacto funcional conectado a Formspree.

---

## 📁 Estructura del Repositorio

```text
proyecto-final-ecommerce-Gonzalo-Orellana/
│
├── index.html              # Página de inicio / tienda principal
├── README.md               # Documentación del proyecto
│
├── pages/                  # Subpáginas del sitio (Arquitectura Multi-Página)
│   ├── productos.html      # Catálogo completo con filtro por categorías
│   └── contacto.html       # Formulario de contacto dedicado
│
├── css/                    # Hojas de estilo externas
│   ├── styles.css          # Estilos globales, layout, header, footer y componentes
│   ├── productos.css       # Estilos específicos del banner y filtros de productos
│   └── contacto.css        # Estilos específicos de la página de contacto
│
└── img/                    # Activos visuales y multimedia
```

---

## 🛠️ Tecnologías y Criterios Técnicos

1. **HTML5 Semántico (100% puro, sin JavaScript):**
   - Etiquetas semánticas: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<blockquote>`, `<footer>`.
   - Cero scripts o librerías dinámicas (cumplimiento estricto con el alcance de la etapa HTML/CSS).
   - Formulario de contacto con campos tipados y validación nativa (`required`, `type="email"`, etc.).

2. **CSS3 Modular y Moderno:**
   - Hoja de estilos externa enlazada mediante `<link rel="stylesheet">`.
   - Cero estilos inline (`style=""`) y cero bloques `<style>`.
   - **Flexbox:** Distribución flexible para header, barras de navegación y tarjetas de productos (`display: flex`, `flex-wrap: wrap`, `gap`).
   - **CSS Grid:** Grillas responsivas para categorías y testimonios (`display: grid`, `repeat(auto-fit, minmax(...))`).
   - Diseño completamente responsivo mediante Media Queries.

3. **Recursos y Tipografía:**
   - **Google Fonts:** Tipografía futurista *Michroma* para títulos y marcas, combinada con *Plus Jakarta Sans* y *DM Sans* para legibilidad óptima.
   - **Font Awesome:** Íconos vectoriales para elementos de interfaz.
   - **Formspree:** Endpoint POST para recepción de correos desde `pages/contacto.html` sin backend.

---