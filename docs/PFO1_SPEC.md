# PFO1 — Landing de Portafolio Personal
## Documento Maestro de Especificacion

> **Estado:** EN PROGRESO  
> **Ultima actualizacion:** 11/08/2026  
> **Fase actual:** Analisis y definicion de arquitectura  
> **Entrega:** 24/08/2026

---

## 1. Contexto del proyecto

### 1.1 Que es esto

Proyecto Formativo Obligatorio 1 (PFO1) de la materia Desarrollo de Sistemas Web — Front End, 2do cuatrimestre 2026. Consiste en una landing page de portafolio personal construida con **HTML y CSS puros** (sin frameworks, sin JavaScript obligatorio).

### 1.2 Restricciones duras

- Solo HTML + CSS. No se requiere JavaScript.
- Entrega: un unico enlace a un repositorio publico de GitHub.
- Deploy obligatorio en Vercel con URL funcional.
- README.md completo con: descripcion, URL de Vercel, decisiones de diseno, y declaracion de uso de IA.
- Enlace visible y funcional al perfil de GitHub dentro de la landing.
- Fecha limite: **24/08/2026**.

### 1.3 Pipeline de trabajo

| Fase | Herramienta | Plan | Estado |
|---|---|---|---|
| Analisis y documentacion | Claude Opus 4.6 (Anthropic) — esfuerzo alto | Pro $20 USD/mes | EN CURSO |
| Diseno de mockups | Figma + plugin Scripter | [DEFINIR] | PENDIENTE |
| Desarrollo | Google Antigravity 2.0 | [DEFINIR] | PENDIENTE |
| Deploy | Vercel | Gratuito (Hobby) | PENDIENTE |
| Documentacion final | Manual | — | PENDIENTE |

### 1.4 Declaracion de uso de IA (borrador para README)

- **Herramientas:** Claude Opus 4.6 (Anthropic) para analisis, arquitectura, documentacion y diseno de mockups; Google Antigravity 2.0 para desarrollo asistido.
- **Plan:** Claude Pro ($20 USD/mes), configuracion de esfuerzo alto. Antigravity [DEFINIR — gratuito/pago y cual].
- **Experiencia previa:** 3 anios estudiando programacion. Experiencia en HTML/CSS puro, React, JavaScript, C#, MySQL, Firebase, MongoDB. Conocimiento en constante evolucion dentro de una tecnicatura en desarrollo de software. Uso habitual de herramientas de IA generativa para desarrollo asistido y co-creacion.
- **Que revise y adapte:** [SE COMPLETARA al finalizar el desarrollo — documentar decisiones propias, correcciones al codigo generado, y criterio aplicado].

---

## 2. Arquitectura de informacion

### 2.1 Estructura de secciones

```
<header>
  └── <nav> — Navegacion fija con links ancla a cada seccion + enlace a GitHub
</header>

<main>
  ├── <section id="hero"> — Presentacion: nombre, apellido, headline, sobre mi
  ├── <section id="habilidades"> — Tech stack con iconos de tecnologias
  ├── <section id="proyectos"> — Galeria de 3 proyectos (seccion personal a eleccion)
  └── <section id="contacto"> — Formulario de contacto con labels
</main>

<footer>
  └── Links secundarios (GitHub, LinkedIn), copyright
</footer>
```

### 2.2 Justificacion de secciones

La consigna pide: nombre/apellido, presentacion, habilidades, contacto, y una **seccion personal a eleccion**. La seccion de **Proyectos** cumple el rol de seccion personal: es una decision deliberada porque la mejor carta de presentacion de un desarrollador es su trabajo concreto. Esto se documenta en el README como decision con criterio propio.

### 2.3 Contenido por seccion

#### Hero / Presentacion
- **H1:** Lucas Luccaroni
- **Headline (subtitulo):** Desarrollador Full Stack
- **Foto de perfil:** Imagen circular, posicionada a la derecha del bloque de texto en desktop. Placeholder circular en el mockup, se reemplaza con la foto real en desarrollo.
- **Layout hero:** Flexbox horizontal en desktop (texto izquierda, foto derecha). Stack vertical centrado en mobile (foto arriba, texto abajo).
- **Parrafo de presentacion:**
  > AI-Driven Developer con foco en sistemas tradicionales e inteligencia artificial aplicada. Experiencia en desarrollo agéntico y co-creación Humano-IA. Desarrollo soluciones a medida, adaptando stack y arquitectura a lo que cada proyecto necesita.
  
  *(Nota: este texto es una version editada para el hero. El contenido tecnico detallado — SQL, NoSQL, BaaS, REST APIs, MVC, RAG, FAISS, modelos cuantizados — se distribuye entre la seccion de Habilidades y las descripciones de proyectos donde se aplicaron.)*
- **CTA principal:** Link a seccion de proyectos ("Ver proyectos")
- **CTA secundario:** Link a GitHub ("GitHub")
- **Enlace visible a GitHub:** https://github.com/lucasluccaroni (requisito obligatorio de la consigna)

#### Habilidades / Tech Stack
- Iconos de tecnologias agrupados por categoria:
  - **Frontend:** HTML, CSS, JavaScript, React
  - **Backend:** Node.js, Express, C#, .NET, REST APIs, MVC
  - **Bases de datos:** MySQL, Firebase, MongoDB, Supabase
  - **IA aplicada:** Ollama, Groq, Openrouter, FAISS, RAG Pipelines, IA-Local
- Iconos en **grayscale por defecto**, transicion a **color original en hover**
- Sin barras de porcentaje (decision estetica: son arbitrarias y poco informativas)
- El bloque de IA aplicada tiene tratamiento visual diferenciado: borde en accent, tags con fondo accent sutil
- **Tecnologias omitidas deliberadamente de la landing** (estan en el CV pero saturarian la grilla): Kotlin/Android Studio, JWT, Bcrypt, Stripe, Twilio, Nodemailer, Swagger, Python, Postman, Git/npm/pnpm. La landing muestra el stack principal; el CV completo cubre el detalle

#### Proyectos (seccion personal a eleccion)
- 3 proyectos con layout jerarquico:
  - **Proyecto estrella (fila completa):** Sistema de gestion web para bar + asistente IA
  - **Proyecto 2 (media fila):** Pagina web tipo e-commerce para muebleria
  - **Proyecto 3 (media fila):** Sistema de gestion de escritorio para gimnasio (C# .NET)
- Cada card contiene: captura de pantalla (con `alt`), titulo, stack tecnologico (badges), descripcion breve, link al repo/deploy

#### Contacto
- Formulario con campos: nombre, email, mensaje
- Cada `<input>` y `<textarea>` con `<label>` asociado (requisito tecnico)
- Boton de envio estilizado
- Nota: el formulario no necesita backend funcional, solo estructura semantica
- **Email de contacto visible:** luccaroni@gmail.com (o lucas_luccaroni@hotmail.com.ar)

#### Footer
- Enlace a GitHub: https://github.com/lucasluccaroni
- Enlace a LinkedIn: https://www.linkedin.com/in/lucas-jose-luccaroni
- Copyright con anio (2026)
- Texto minimo, tratamiento visual discreto

---

## 3. Sistema de diseno

### 3.1 Paleta de colores — CONFIRMADA

**Direccion cromatica:** Blue Steel + Cream calido. Inspirada en Sherwin Williams Bunglehouse Blue (SW 0048). El cream (#F0E8D0) tiene temperatura calida tipo "papel antiguo" que armoniza con la tipografia serif editorial. El azul acero desaturado (#5B7F8E) como acento transmite solidez tecnica sin frialdad.

```css
:root {
  /* Fondos */
  --color-bg-primary: #F0E8D0;       /* Cream calido — fondo principal */
  --color-bg-secondary: #F6F1E4;     /* Cream mas claro — secciones alternas */
  --color-bg-card: #FAF8F0;          /* Casi blanco calido — superficie de cards */
  --color-bg-dark: #2C3E4A;          /* Azul oscuro — footer, secciones invertidas */

  /* Texto */
  --color-text-primary: #2C3E4A;     /* Azul oscuro — texto principal */
  --color-text-secondary: #4A5E6A;   /* Azul gris medio — texto complementario */
  --color-text-light: #7A8E9A;       /* Azul gris claro — captions, metadata */
  --color-text-on-dark: #F0E8D0;     /* Cream — texto sobre fondos oscuros */

  /* Acento */
  --color-accent: #5B7F8E;           /* Blue steel — links, botones, detalles */
  --color-accent-hover: #4A6B78;     /* Blue steel oscuro — estados hover */
  --color-accent-light: rgba(91, 127, 142, 0.12); /* Blue steel al 12% — fondos de tags */

  /* Bordes y separadores */
  --color-border: #D4CFC2;           /* Cream oscuro — lineas sutiles */
  --color-border-hover: #5B7F8E;     /* Acento — bordes en hover */
}
```

**Criterio:** La base cream calida (#F0E8D0) se eligio deliberadamente para complementar la tipografia serif (EB Garamond + Source Serif 4). Los grises frios del planteo inicial generaban tension con el caracter editorial de las fuentes; el cream resuelve esa tension y produce una estetica "paper editorial" coherente. El azul acero se usa con restriccion maxima: solo en links, botones CTA, bordes hover de cards, y un detalle decorativo en el hero. Los colores de texto derivan del azul oscuro en lugar de negro puro, manteniendo la paleta cromaticamente unificada.

### 3.2 Tipografia

```css
/* Google Fonts import */
@import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;0,700;1,400&family=Source+Serif+4:ital,opsz,wght@0,8..60,200..900;1,8..60,200..900&display=swap');

:root {
  --font-heading: 'EB Garamond', Georgia, 'Times New Roman', serif;
  --font-body: 'Source Serif 4', Georgia, 'Times New Roman', serif;

  /* Escala tipografica con clamp() para fluidez */
  --text-hero: clamp(2.5rem, 5vw + 1rem, 4.5rem);
  --text-h1: clamp(2rem, 3vw + 0.5rem, 3rem);
  --text-h2: clamp(1.5rem, 2vw + 0.5rem, 2.25rem);
  --text-h3: clamp(1.125rem, 1.5vw + 0.25rem, 1.5rem);
  --text-body: clamp(1rem, 0.5vw + 0.875rem, 1.125rem);
  --text-small: clamp(0.8125rem, 0.25vw + 0.75rem, 0.875rem);
  --text-caption: 0.75rem;
}
```

**Justificacion:** EB Garamond para headings aporta peso visual y tradicion tipografica que transmite seriedad profesional. Source Serif 4 para body esta optimizada por Adobe para lectura en pantalla, con rango de pesos de 200 a 900 que permite jerarquia sin cambiar de familia. Ambas son serif, pero con personalidades complementarias: Garamond es clasica-humanista, Source Serif es contemporanea-funcional. Los fallbacks (Georgia, Times New Roman) garantizan coherencia si Google Fonts falla.

### 3.3 Espaciado

```css
:root {
  --space-xs: 0.5rem;    /* 8px */
  --space-sm: 1rem;      /* 16px */
  --space-md: 1.5rem;    /* 24px */
  --space-lg: 2rem;      /* 32px */
  --space-xl: 3rem;      /* 48px */
  --space-2xl: 4rem;     /* 64px */
  --space-section: clamp(4rem, 8vw, 8rem);  /* Separacion entre secciones */
}
```

### 3.4 Bordes y sombras

```css
:root {
  --radius-sm: 4px;      /* Bordes sutiles, no redondeados */
  --radius-md: 8px;      /* Cards */
  --shadow-card: 0 1px 3px rgba(44, 62, 74, 0.06), 0 1px 2px rgba(44, 62, 74, 0.04);
  --shadow-card-hover: 0 4px 12px rgba(44, 62, 74, 0.08), 0 2px 4px rgba(44, 62, 74, 0.04);
}
```

**Criterio:** Radios minimos para mantener el tono editorial. Las sombras usan el azul oscuro de la paleta (rgba derivado de #2C3E4A) en lugar de negro puro, para que se integren con la calidez del cream. Sombras sutiles para no competir con la tipografia como protagonista visual.

---

## 4. Maquetacion y layout

### 4.1 Estrategia: Flexbox + Grid

| Seccion | Tecnologia | Justificacion |
|---|---|---|
| Nav | Flexbox | Distribucion lineal de items en un eje. `justify-content: space-between` para logo/links. |
| Hero | Flexbox | Centrado vertical y horizontal de contenido textual. Una sola dimension. |
| Habilidades | Grid | Grilla de iconos con cantidades variables. `grid-template-columns: repeat(auto-fit, minmax(80px, 1fr))`. |
| Proyectos | Grid | Layout asimetrico: proyecto estrella ocupa fila completa, otros dos comparten fila. `grid-column: span 2` para el destacado. |
| Contacto | Flexbox | Formulario con campos apilados verticalmente. Estructura lineal. |
| Footer | Flexbox | Distribucion de links y copyright en un eje. |

**Justificacion para README:** Se utiliza Flexbox para componentes de distribucion lineal (un solo eje: nav, hero, footer, formulario) y Grid para layouts bidimensionales con multiples items de tamano controlado (habilidades, proyectos). La combinacion aprovecha las fortalezas de cada tecnologia donde corresponde, en lugar de forzar una sola solucion para todo.

### 4.2 Responsive

- **Mobile first** como base del CSS.
- Breakpoints:
  - `768px` — tablet: grilla de proyectos pasa de 1 columna a 2.
  - `1024px` — desktop: layout completo con proyecto estrella en fila propia.
- Max-width del contenedor: `1200px` con `margin: 0 auto`.
- Unidades relativas en todo: `rem`, `%`, `fr`, `clamp()`, `min()`, `max()`.
- Imagenes con `max-width: 100%` y `height: auto`.

---

## 5. Interactividad y animaciones (CSS puro)

### 5.1 Transiciones (hover/focus)

```css
/* Botones y links */
transition: color 0.3s ease, background-color 0.3s ease, border-color 0.3s ease;

/* Cards de proyectos */
transition: transform 0.3s ease, box-shadow 0.3s ease;
/* En hover: transform: translateY(-4px) + shadow mas pronunciada */

/* Iconos de tecnologias */
filter: grayscale(1);
transition: filter 0.4s ease;
/* En hover: filter: grayscale(0) — se revela el color original */
```

### 5.2 Animaciones con @keyframes

```css
/* Fade-in del hero al cargar la pagina */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.hero-content {
  animation: fadeInUp 0.8s ease forwards;
}

/* Animacion escalonada para items del hero */
.hero-content > *:nth-child(1) { animation-delay: 0.1s; }
.hero-content > *:nth-child(2) { animation-delay: 0.25s; }
.hero-content > *:nth-child(3) { animation-delay: 0.4s; }
```

### 5.3 Scroll-driven animations (mejora progresiva)

```css
/* Fade-in de cards al entrar en viewport — CSS puro, sin JS */
/* Solo navegadores con soporte (Chrome 115+, Edge 115+) */
@keyframes fadeInOnScroll {
  from { opacity: 0; transform: translateY(30px); }
  to { opacity: 1; transform: translateY(0); }
}

.project-card {
  animation: fadeInOnScroll linear both;
  animation-timeline: view();
  animation-range: entry 0% entry 30%;
}

/* FALLBACK: los elementos son visibles por defecto */
/* La animacion es mejora progresiva, no depende de ella */
```

### 5.4 Accesibilidad de animaciones

```css
/* Respetar preferencias del usuario */
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

---

## 6. Accesibilidad y semantica avanzada

### 6.1 HTML semantico con comentarios explicativos

Se incluiran al menos **4 comentarios HTML explicativos** (requisito de rubrica "Propone"):

1. Antes del `<nav>`: explicando la estructura de navegacion y el uso de anclas.
2. Antes de la seccion de proyectos: explicando por que es la seccion personal a eleccion.
3. Antes del formulario: explicando la asociacion label-input.
4. Antes del footer: explicando la redundancia intencional del enlace a GitHub.

### 6.2 Roles ARIA pertinentes

```html
<nav aria-label="Navegacion principal">
<section id="proyectos" aria-labelledby="proyectos-titulo">
<form aria-label="Formulario de contacto">
<input aria-describedby="email-help">
```

**Criterio:** ARIA solo donde agrega valor para lectores de pantalla, no decorativo. Esto cubre "Supera" en estructura semantica.

### 6.3 Atributos alt

Todas las imagenes llevan `alt` descriptivo del contenido, no generico. Ejemplo: `alt="Captura de pantalla del sistema de gestion para bar mostrando el panel de asistente IA"` en lugar de `alt="proyecto 1"`.

---

## 7. Estructura de archivos

```
pfo1-portfolio/
├── index.html
├── css/
│   └── styles.css
├── assets/
│   ├── img/
│   │   ├── proyecto-bar-ia.webp
│   │   ├── proyecto-muebleria.webp
│   │   ├── proyecto-gimnasio.webp
│   │   └── tech-icons/
│   │       ├── html.svg
│   │       ├── css.svg
│   │       ├── javascript.svg
│   │       ├── react.svg
│   │       ├── csharp.svg
│   │       ├── dotnet.svg
│   │       ├── mysql.svg
│   │       ├── firebase.svg
│   │       └── mongodb.svg
│   └── fonts/                    (si se descargan localmente en vez de CDN)
├── README.md
└── .gitignore
```

---

## 8. Mapeo de rubrica → implementacion

| Criterio | Nivel objetivo | Que implementamos |
|---|---|---|
| Estructura semantica | **Supera** | header/nav/main/footer + section/article + 4 comentarios explicativos + ARIA pertinentes + alt descriptivos |
| Maquetacion | **Supera** | Flexbox + Grid combinados + justificacion tecnica en README + unidades relativas + responsive fluido |
| Estilizacion | **Supera** | Variables CSS (custom properties) + 2 familias Google Fonts serif con justificacion + jerarquia tipografica con clamp() |
| Interactividad | **Supera** | Transiciones en hover/focus + @keyframes personalizados (fadeInUp) + scroll-driven animation como mejora progresiva + prefers-reduced-motion |
| Documentacion | **Supera** | Commits con Conventional Commits + README con decisiones justificadas + declaracion de IA completa + historial organizado |

---

## 9. Proyectos a mostrar

### Proyecto estrella — SAO Bar - Sistema de Gestión
- **Tipo:** Aplicacion web full-stack con IA integrada
- **Periodo:** Abril 2026 - Julio 2026
- **Stack:** Next.js, TypeScript, Tailwind CSS, Supabase (PostgreSQL)
- **Modulos:** ABM de productos, Comandas, Caja del dia, Cierre de caja, Historial y reportes, Calculadora de costos, Niveles de usuarios
- **IA:** Asistente IA incorporado con RAG + Tool Use (LangGraph, Ollama, FAISS, Nomic Embed)
- **Descripcion para la card:** Sistema de gestion integral para un bar con asistente de inteligencia artificial incorporado. ABM de productos, comandas, caja, reportes y calculadora de costos. Implementacion de asistente IA con pipeline RAG y Tool Use.
- **Link:** [URL de SAO Bar — CONFIRMAR]
- **Captura:** [PENDIENTE]
- **Tratamiento visual:** Fila completa en la grilla (grid-column: span 2), captura mas grande, descripcion extendida. Badges de stack: Next.js, TypeScript, Tailwind, Supabase, RAG/IA.

### Proyecto 2 — Parben Home
- **Tipo:** Sitio web responsive full-stack (freelance)
- **Periodo:** Enero 2025 - Marzo 2025
- **Stack:** React, Vite, HTML, CSS, JavaScript, Firebase (base de datos + mailing)
- **Descripcion para la card:** Sitio web responsive para Parben Home, empresa de diseno de interiores. Frontend en React con Vite, backend en Firebase para base de datos y sistema de mailing.
- **Link:** [URL de Parben Home — CONFIRMAR]
- **Captura:** [PENDIENTE]
- **Tratamiento visual:** Media fila en grilla (1 de 2 cards). Badges de stack: React, Vite, JavaScript, Firebase.

### Proyecto 3 — Sistema de gestion para gimnasio
- **Tipo:** Aplicacion de escritorio
- **Periodo:** Agosto 2025 - Noviembre 2025
- **Stack:** C#, .NET Framework, MySQL
- **Descripcion para la card:** Aplicacion de escritorio para la gestion integral de un gimnasio. ABM de socios, abonados y actividades. Desarrollado con C# .NET Framework y base de datos MySQL.
- **Link:** [COMPLETAR si hay repo]
- **Captura:** [PENDIENTE]
- **Tratamiento visual:** Media fila en grilla (1 de 2 cards). Badges de stack: C#, .NET, MySQL.

---

## 10. Pendientes por definir

- [x] **Paleta de colores**: Blue Steel + Cream calido (confirmada)
- [x] **Tipografia**: EB Garamond (headings) + Source Serif 4 (body) (confirmada)
- [x] **Nombre y apellido**: Lucas Jose Luccaroni
- [x] **URL del perfil de GitHub**: https://github.com/lucasluccaroni
- [x] **Headline profesional**: "Desarrollador Full Stack"
- [x] **Parrafo de presentacion**: Confirmado con frase final "soluciones a medida"
- [x] **Stacks tecnologicos** de cada proyecto (confirmados y enriquecidos con CV)
- [x] **Plan de IA**: Claude Pro $20 USD/mes, Opus 4.6 esfuerzo alto. Antigravity pendiente.
- [x] **Datos de contacto**: luccaroni@gmail.com, LinkedIn: lucas-jose-luccaroni
- [ ] **Links** a deploys de SAO Bar y Parben Home (confirmar URLs exactas)
- [ ] **Capturas de pantalla** de los 3 proyectos
- [ ] **Foto de perfil** (la del CV o una nueva)
- [ ] **Diseno en Figma**: Script 1 (Hero) OK, Script 2 (Habilidades) en prueba, Scripts 3-4 pendientes

---

## 11. Estrategia de commits

Usar Conventional Commits para que el historial cuente la historia del desarrollo:

```
1.  feat: init project structure and base HTML
2.  feat: add hero section with semantic markup
3.  feat: add skills section with tech icons grid
4.  feat: add projects section with card layout
5.  feat: add contact form with labels
6.  feat: add header nav and footer
7.  style: implement CSS variables and color system
8.  style: add Google Fonts and typography scale
9.  style: implement Flexbox layout for nav and hero
10. style: implement Grid layout for skills and projects
11. style: add responsive breakpoints
12. style: add transitions and hover effects
13. style: add keyframe animations
14. a11y: add ARIA roles and descriptive alt texts
15. docs: add HTML explanatory comments
16. docs: complete README with decisions and AI declaration
17. deploy: configure and publish to Vercel
```

**Nota:** Esta es una guia orientativa. Los commits reales deben reflejar el proceso real, no fabricarse al final.

---

*Este documento se actualiza a medida que avanza el proyecto. Cada decision queda registrada con su justificacion para alimentar tanto al README final como a la IA de desarrollo (Antigravity).*
