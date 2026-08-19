# Portafolio Personal — Lucas Luccaroni
## Proyecto Formativo Obligatorio 1 (PFO1) — Desarrollo de Sistemas Web Front End
> **Tecnicatura Superior en Desarrollo de Software (IFTS) — 2do Cuatrimestre 2026**  
> **Estudiante:** Lucas José Luccaroni  
> **Repositorio GitHub:** [ifts-frontend-pfo1-luccaroni-lucas](https://github.com/lucasluccaroni/ifts-frontend-pfo1-luccaroni-lucas)  
> **Despliegue Vercel:** [https://ifts-frontend-pfo1-luccaroni-lucas.vercel.app](https://ifts-frontend-pfo1-luccaroni-lucas.vercel.app) *(Deploy activo)*

---

## 1. Descripción del Proyecto

Landing page de portafolio profesional desarrollada con **HTML5 semántico y CSS3 puro** (sin frameworks de JavaScript ni dependencias de compilación). El sitio expone mi perfil como **AI-Driven Developer** y **Desarrollador Full Stack**, destacando una selección de sistemas reales desarrollados (web, desktop e IA aplicada) con un enfoque estético de tipo editorial y altos estándares de accesibilidad y diseño adaptativo.

---

## 2. Documentos Complementarios de Análisis y Metodología

> [!IMPORTANT]
> **Lectura Indispensable para la Evaluación del Proyecto:**  
> La comprensión cabal del análisis, las decisiones de arquitectura y la metodología de desarrollo agéntico no se agota únicamente en el código fuente o en este resumen ejecutivo del `README.md`. Es **estrictamente menester** examinar los documentos complementarios almacenados en el directorio `docs/` para ponderar el trasfondo analítico, la fundamentación del sistema de diseño y la trazabilidad completa del proyecto.

Dentro de la carpeta `docs/` se destacan dos archivos fundamentales que respaldan el proceso metodológico y arquitectónico del proyecto:

* **[PFO1_SPEC.md](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/docs/PFO1_SPEC.md):** Documento maestro de especificación técnica resultante de la **Fase 1 (Análisis y Documentación Arquitectónica)**. Registra la investigación previa, la justificación cromática, el diseño del sistema de tipografía editorial, la definición de contenido por sección y el mapeo conceptual inicial.
* **[estado_actual.md](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/docs/estado_actual.md):** Hoja de ruta dinámica e incremental utilizada durante todo el ciclo de desarrollo. Registra el progreso hito por hito (setup, maquetación semántica, sistema CSS, assets e integración), garantizando la trazabilidad metodológica y el relevo agéntico.

---

## 3. Matriz de Cumplimiento de Rúbrica de Evaluación (Nivel "Supera")

A continuación se detalla la trazabilidad técnica de cada criterio evaluado en la consigna del proyecto, señalando las ubicaciones exactas dentro del código fuente donde se evidencia el nivel máximo de desempeño (**Supera**):

| Criterio de Evaluación | Nivel Alcanzado | Evidencia Técnica y Ubicación en Código Fuente |
|---|---|---|
| **Estructura HTML y Semántica** | **Supera** | - Uso riguroso de etiquetas semánticas maestras (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`) en [index.html](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/index.html).<br>- Atributos ARIA explícitos y pertinentes (`aria-label`, `aria-labelledby`, `aria-hidden="true"`).<br>- Atributos `alt` contextuales completos en todas las imágenes.<br>- **4 comentarios normativos explicativos** incluidos en el HTML (ver detalle abajo). |
| **Maquetación y Layout (Flexbox / Grid)** | **Supera** | - Distribución 1D con **Flexbox** en cabecera, hero, formulario y footer.<br>- Distribución 2D adaptativa con **CSS Grid** en la sección de habilidades y en proyectos.<br>- **Layout Asimétrico Jerárquico**: El Proyecto Estrella (*SAO Bar*) abarca la fila completa (`grid-column: 1 / -1`) en escritorio en [styles.css](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/css/styles.css#L446-L453).<br>- Maquetación responsive basada en unidades relativas (`rem`, `%`, `clamp()`, `fr`). |
| **Estilización y Sistema de Diseño** | **Supera** | - Sistema completo de **Custom Properties** (`:root`) en [styles.css](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/css/styles.css#L1-L45) con paleta Blue Steel + Cream cálido.<br>- **2 familias tipográficas serif de Google Fonts** (`EB Garamond` para títulos y `Source Serif 4` para lectura).<br>- Escala tipográfica fluida implementada con **`clamp()`** para adaptación responsiva. |
| **Interactividad y Animaciones** | **Supera** | - Transiciones suaves en `:hover` y `:focus` en botones y tarjetas.<br>- Animaciones `@keyframes fadeInUp` con delays escalonados en la sección Hero.<br>- Micro-interacción zoom suave (`transform: scale(1.04)`) en capturas de proyectos.<br>- **Accesibilidad de Movimiento**: Bloque `@media (prefers-reduced-motion: reduce)` en [styles.css](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/css/styles.css#L690-L700) para inhabilitar movimiento en usuarios sensibles. |
| **Documentación y Repositorio** | **Supera** | - Historial de commits estructurado con Conventional Commits.<br>- Bitácora de seguimiento incremental en [docs/estado_actual.md](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/docs/estado_actual.md).<br>- `README.md` exhaustivo con decisiones justificadas y declaración de IA. |

---

## 4. Ubicación de los Comentarios HTML Normativos

Conforme a los requerimientos del nivel "Supera", se incluyeron **4 comentarios explicativos** en [index.html](file:///d:/repositorios/tecnicatura-desarrollo-software/frontend-pfo1-landing-page/index.html):

1. **Comentario 1 (Estructura de Navegación):** Ubicado sobre la etiqueta `<header>` (Líneas 21-29). Explica la arquitectura de la barra de navegación, el uso de enlaces ancla para desplazamiento interno y la inclusión visible del perfil de GitHub.
2. **Comentario 2 (Sección Personal a Elección):** Ubicado antes de `<section id="proyectos">` (Líneas 150-157). Justifica deliberadamente la elección de la sección "Proyectos Destacados" como la mejor demostración práctica de competencias técnicas para un desarrollador.
3. **Comentario 3 (Asociación Label-Input):** Ubicado antes de `<section id="contacto">` (Líneas 261-268). Detalla la asociación explícita mediante el atributo `for` de cada `<label>` con el `id` de su respectivo `<input>` o `<textarea>` para cumplir estándares de accesibilidad WCAG.
4. **Comentario 4 (Redundancia Intencional en Footer):** Ubicado sobre la etiqueta `<footer>` (Líneas 307-314). Justifica la repetición del enlace visible a GitHub al cierre de la página como buena práctica de usabilidad y cumplimiento de consigna.

---

## 5. Decisiones de Arquitectura y Sistema de Diseño

### Paleta de Colores (Blue Steel + Cream Cálido)
La dirección cromática combina un **Cream cálido** (`#F0E8D0`) como superficie principal con un **Azul Acero** (`#5B7F8E`) como tono de acento y un **Azul Oscuro** (`#2C3E4A`) para contraste tipográfico. Esta elección rompe con los grises fríos genéricos, transmitiendo una estética tipo "papel editorial" sofisticada que evoca seriedad técnica y legibilidad.

### Tipografía Serif Editorial
Se seleccionaron dos familias de **Google Fonts**:
* **EB Garamond:** Aplicada en los encabezados (`<h1>`, `<h2>`, `<h3>`), aporta elegancia y jerarquía visual.
* **Source Serif 4:** Diseñada por Adobe y optimizada para pantallas, se utiliza en el texto de cuerpo ofreciendo alta legibilidad.
* **Jerarquía con `clamp()`:** Permite que los tamaños de fuente escalen de forma continua entre dispositivos móviles y de escritorio sin saltos bruscos.

### Híbrido Flexbox + CSS Grid
Se aplicó la regla de dimensionalidad en CSS: **Flexbox** para componentes unidimensionales (alineación en un solo eje) y **CSS Grid** para estructuras bidimensionales. El grid de proyectos es asimétrico, otorgando jerarquía visual al proyecto estrella (*SAO Bar*) al extenderse en el ancho completo del contenedor.

---

## 6. Declaración de Co-creación Humano-IA

En cumplimiento con la política de transparencia académica del IFTS y las directivas de evaluación:

* **Herramientas de IA Utilizadas:** Anthropic Claude (Opus 4.6) para arquitectura, análisis pedagógico y estructuración de documentación; Google Antigravity 2.0 como asistente de código.
* **Plan y Contexto:** Uso de entornos agénticos configurados con reglas estrictas de seguridad (sin acceso a credenciales locales, sin emojis, control exclusivo de Git por parte del alumno).
* **Supervisión y Criterio Humano:** El alumno (Lucas Luccaroni) definió el concepto estético, seleccionó los proyectos a exhibir, cargó y estructuró las capturas multimedia, aprobó cada bloque de código CSS/HTML generado, probó la responsividad y ejecutó manualmente cada commit y push al repositorio remoto de GitHub.

---

## 7. Estructura del Repositorio

```
frontend-pfo1-landing-page/
├── index.html                  # Maquetación HTML5 semántica principal
├── css/
│   └── styles.css              # Sistema de diseño, Custom Properties y responsive
├── assets/
│   └── img/                    # Capturas de pantalla, foto de perfil y recursos
│       ├── perfil-lucas.png
│       ├── sao-bar/            # Capturas del sistema SAO Bar (Proyecto 1)
│       ├── parben-home/        # Capturas del sitio Parben Home (Proyecto 2)
│       └── gym/                # Capturas del sistema Gimnasio (Proyecto 3)
├── docs/
│   ├── PFO1_SPEC.md            # Documento maestro de especificación técnica
│   ├── estado_actual.md        # Bitácora incremental de desarrollo y relevo
│   └── pfo1-consigna-2026.pdf  # Consigna oficial de la materia
```

---

## 8. Revisión / Adaptación de mi Criterio

En todas las etapas que constituyen la premisa, el analisis, la documentacion, el desarrollo y la puesta a punto de un desarrollo de software intervengo directa y activamente junto con la herramienta de IA que esté utilizando en ese momento. Es la clave de la colaboración humano-IA Co-Work. Me desenvuelvo en una metodología de pensamiento colaborativo donde la IA se encarga del razonamiento, ya que sin duda es mil veces mejor que yo, y yo me encargo de la imaginación, la creatividad, la visión macro del proyecto, el marco, los límites y las reglas del flujo de la información, aporto mi criterio residual humano para evaluar los resultados, proponer y buscar alternativas y ajustar las devoluciones de la IA para que se adapten a lo que yo quiero, a lo que yo necesito. Ejemplos de esto son documentación viva compartida entre modelos, reglas de comportamiento, límites y reportes, planes de ruta, iteraciones en las respuestas de la ia corrigiendo bugs en la pagina, contenedores mal ajustados, fallos en el apartado responsive, etc. La intervención que tengo en este proyecto es absoluta, ya que todo lo que está escrito lo hizo la IA, pero cómo lo escribió, donde lo escribió, cómo se organizó, todas las decisiones de estilo y diseño, la arquitectura de carpetas, etc, fue mi intervención y mi criterio aplicado al proyecto.