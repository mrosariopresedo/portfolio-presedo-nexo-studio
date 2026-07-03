# Portfolio Personal · María del Rosario Presedo Valenzuela

Sitio web personal de Rosario Presedo, desarrollado para la materia Diseño y Desarrollo Web 1 - Comisión 26 (2026).

**Sitio publicado:** https://mrosariopresedo.github.io/portfolio-presedo-nexo-studio/  
**Integrante de:** [Nexo Studio](https://mrosariopresedo.github.io/nexo-studio/) · Grupo 02 · DDW1C26

---

## 1. Estructura del sitio

```
.
├── index.html        → Inicio: sobre mí, competencias y Nexo Studio
├── intereses.html    → Intereses y filosofía personal
├── contacto.html     → Correo y disponibilidad
├── styles/
│   └── styles.css    → Estilos personalizados (patrón cuaderno, animaciones)
└── img/
    └── infografia.jpg
```

**Mapa del sitio:**

```
Inicio (index.html)
├── Intereses (intereses.html)
└── Contacto (contacto.html)
```

---

## 2. Descripción de páginas

### Inicio (`index.html`)
Página principal con presentación personal. Incluye un hero con nombre en tipografía manuscrita, sección "Sobre mí" con descripción del perfil profesional, sección de competencias con cards y un bloque que enlaza al sitio grupal de Nexo Studio. Termina con un llamado a la acción hacia la página de contacto.

### Intereses (`intereses.html`)
Sección que presenta los intereses personales y la filosofía de trabajo. Contenido redactado en primera persona con el estilo visual del cuaderno que caracteriza al sitio.

### Contacto (`contacto.html`)
Página de contacto vía `mailto:`, sin formulario. Presenta una tarjeta con el correo principal y enlaces `mailto:` (correo directo y "agendar charla"), una tarjeta con la disponibilidad horaria y un bloque que enlaza al sitio de Nexo Studio.

---

## 3. Estética y concepto de diseño

El sitio adopta una estética de **cuaderno escolar / diario personal**: fondo papel crema con líneas horizontales, tipografía manuscrita, elementos decorativos como post-its, washi tape, doodles a mano y marcos de polaroid. La propuesta fue diseñar algo con personalidad propia y reconocible, que se diferencie de un portfolio genérico.

---

## 4. Contenido de la materia aplicado

Esta sección documenta cómo el sitio aplica los conceptos enseñados en Diseño y Desarrollo Web 1 (DDW1C26 - UADE, 2026).

---

### 4.1 Leyes de Gestalt y principios de diseño visual

**Proximidad**
Cada card de competencias agrupa ícono, título y descripción como una unidad visual. Los elementos del footer (nombre y filiación a la izquierda, correo y Nexo Studio a la derecha) se organizan en dos bloques claramente separados.

**Similitud**
Las cards de competencias tienen la misma estructura (ícono + título manuscrito + descripción), con variaciones de color y ángulo que las diferencian sin romper la coherencia del conjunto. Los post-its en la sección "Sobre mí" siguen el mismo patrón.

**Figura y fondo**
El fondo de papel crema actúa como base unificadora sobre la que descansan los elementos (cards, post-its, polaroid). Esta relación figura-fondo es parte del concepto: todo parece pegado sobre un cuaderno físico.

**Cierre**
El logo "MRPV." funciona como sigla cerrada y reconocible. El punto final en rojo cierra visualmente la marca personal y actúa como sello de identidad.

**Pregnancia (buena forma)**
La interfaz usa formas simples y reconocibles (rectángulos, post-its, marcos de polaroid) que el usuario interpreta de inmediato sin necesidad de explicación.

**Contraste (CRAP)**
Se genera contraste entre la tipografía manuscrita de gran tamaño en los títulos y la tipografía más pequeña y regular en los párrafos. El color rojo de los detalles (punto del logo, líneas de margen) contrasta con el fondo crema y orienta la mirada.

**Repetición (CRAP)**
El mismo fondo de papel, las mismas familias tipográficas y los mismos colores se repiten en las tres páginas. Los elementos decorativos (líneas del cuaderno, numeración de secciones, washi tape) se repiten de manera consistente, reforzando la identidad visual del sitio.

**Alineación (CRAP)**
El contenido principal está alineado a un contenedor de ancho máximo centrado en la página. En pantallas medianas y grandes, el contenido se desplaza hacia la derecha dejando espacio para la columna de perforaciones del cuaderno, generando un eje de alineación coherente en todas las páginas.

**Jerarquía visual**
El título principal (`<h1>`) en tipografía manuscrita de tamaño muy grande domina visualmente la pantalla al cargar. Los `<h2>` de cada sección son más pequeños, y los `<h3>` dentro de las cards más pequeños aún. Esta progresión de tamaños define la jerarquía de forma clara.

---

### 4.2 Tipografía

Se usaron tres familias tipográficas importadas desde Google Fonts, cada una con un rol específico.

| Familia | Tipo | Uso en el sitio |
|---|---|---|
| **Caveat** | Manuscrita | Títulos, logo, nombre de secciones |
| **Newsreader** | Serif | Párrafos y texto de cuerpo |
| **JetBrains Mono** | Monoespaciada | Detalles técnicos, etiquetas, fechas |

**Decisiones tipográficas:**

- La fuente **manuscrita** (Caveat) es la elección más importante del sitio: define el concepto del cuaderno y le da personalidad inmediata al portfolio. Se usa solo en títulos porque las fuentes manuscritas tienen menor legibilidad que las sans-serif en bloques largos de texto pequeño.
- La fuente **serif** (Newsreader) en los párrafos le da al sitio un tono más editorial y personal, diferente del sans-serif que domina en la mayoría de los sitios de tecnología.
- La fuente **monoespaciada** (JetBrains Mono) en detalles técnicos genera contraste tipográfico con las otras dos familias y refuerza el perfil de desarrolladora.
- El **interlineado** (`line-height`) de los párrafos es amplio para facilitar la lectura, siguiendo la recomendación de 1.3 a 1.5 veces el tamaño de la fuente.
- Los títulos `<h1>` tienen un tamaño notablemente mayor al resto, marcando la jerarquía visual desde el primer momento.

---

### 4.3 Teoría del color

La paleta se define mediante variables CSS (custom properties) al inicio de `styles.css` y se expresa en formato **hexadecimal**, lo que permite modificar el tema del sitio desde un único lugar.

| Variable | Valor HEX | Uso |
|---|---|---|
| `--paper` | `#faf3e3` | Fondo principal (el "papel") |
| `--paper-edge` | `#f1e7cf` | Borde del papel / perforaciones |
| `--ink` | `#1f1b17` | Texto principal |
| `--ink-soft` | `#4a3f33` | Texto secundario |
| `--rule` | `#b9cee0` | Líneas horizontales del cuaderno |
| `--margin-red` | `#d94a3d` | Logo, línea de margen, énfasis y foco |
| `--highlight` | `#ffe066` | Resaltado tipo marcador (amarillo) |
| `--marker-pink` | `#ff9bb5` | Marcador alternativo (rosa) |

> El sitio usa un **único tema fijo** (la paleta cálida listada arriba). Todas las variables de color y de tipografía se definen una sola vez en `:root`, al inicio de `styles.css`, de modo que el estilo se puede ajustar desde un único lugar.

**Justificación de las decisiones de color:**

El **fondo crema** evoca el papel físico, que es el concepto central del diseño. El blanco puro (`#FFFFFF`) rompería la ilusión de estar viendo un cuaderno real y genera más fatiga visual en pantalla.

El **rojo** de las líneas de margen es una referencia directa a los cuadernos escolares argentinos, lo que hace que el usuario reconozca el concepto de forma inmediata. Según la psicología del color, el rojo genera atención y energía, lo que lo hace ideal para los detalles de énfasis.

Los colores de los markers (amarillo y rosa) se usan exclusivamente para resaltar palabras clave en el texto. Al usarlos con moderación, conservan su poder de atraer la atención sin saturar el diseño.

La **tinta oscura** en lugar del negro puro (`#000000`) para el texto genera un contraste suficiente con el fondo crema sin la dureza del negro absoluto, acompañando el tono cálido del sitio.

---

### 4.4 HTML semántico

La estructura usa las etiquetas semánticas de HTML5 en lugar de `<div>` genéricos:

```
<header>    → encabezado con el logo y la navegación principal
<nav>       → menú con los tres enlaces del sitio
<main>      → contenido principal de cada página (entre el header y el footer)
<section>   → bloques temáticos: hero, sobre mí, competencias, Nexo Studio, CTA
<article>   → cada card de competencia es una unidad de contenido independiente
<figure>    → la imagen polaroid con su epígrafe (figcaption)
<footer>    → pie de página con correo y datos académicos
<h1>-<h3>   → jerarquía de encabezados sin saltear niveles
<a>         → hipervínculos con href y texto descriptivo
```

El uso de `<figure>` y `<figcaption>` para la imagen principal aplica la semántica correctamente: no es una imagen decorativa, tiene una descripción asociada que la convierte en una figura con epígrafe con sentido propio.

Los elementos decorativos (perforaciones del cuaderno, cintas washi tape) llevan `aria-hidden="true"` para que los lectores de pantalla los ignoren, ya que no aportan información de contenido.

**Buenas prácticas de accesibilidad:**
- `lang="es"` en `<html>`.
- Atributo `alt` descriptivo en la imagen de la infografía.
- `aria-hidden="true"` en todos los elementos puramente decorativos.
- `rel="noopener noreferrer"` en los enlaces externos con `target="_blank"`.
- `<meta name="description">` con descripción propia en cada página.
- Foco de teclado visible mediante `:focus-visible` en navegación, "stickers" y enlaces de texto.
- Contenido principal de cada página envuelto en `<main>`.

**Contacto (`contacto.html`):**
- El contacto se resuelve con enlaces `mailto:`, no hay formulario ni campos de entrada.
- El enlace "agendar charla" usa `mailto:` con un asunto predefinido (`?subject=...`).
- El correo se muestra como texto y como enlace, con `break-words` para que no desborde en pantallas chicas.

---

### 4.5 CSS: modelo de caja, cascada y diseño responsive

**Arquitectura del CSS**

El sitio combina **Tailwind CSS** (desde CDN) para el layout y los espaciados, con el archivo `styles/styles.css` para los estilos que definen la estética del cuaderno: el patrón de líneas del fondo, los post-its, el efecto polaroid, las cintas washi tape y las animaciones de hover.

El CSS propio usa **variables CSS** (custom properties) al inicio del archivo para centralizar todos los colores y fuentes, siguiendo el principio de separación entre estructura (HTML) y presentación (CSS).

**Modelo de caja (Box Model)**

El modelo de caja está presente en todos los componentes:
- Las **cards de competencias** tienen `padding` interno para separar el contenido del borde, y un `border` que simula el borde de una nota de papel.
- Los **post-its** tienen `padding` generoso y `margin` para que no queden pegados entre sí.
- El **contenedor principal** usa el `max-width` y el `margin: auto` de Tailwind (`max-w-5xl mx-auto`) para centrarse, con `padding` lateral que aumenta en pantallas más grandes (`px-6 md:pl-28`).

El espaciado lateral y la centralización del contenedor se resuelven con utilidades de Tailwind. El CSS propio define el modelo de caja de los componentes de la estética cuaderno (cards, post-its, polaroids, cintas, chips, stamps).

**Propiedad `display`**

- Las "perforaciones" del cuaderno (`.holes`) usan `display: flex` con `flex-direction: column` para distribuir los puntos en vertical.
- Los "stickers" (`.sticker`) usan `display: inline-flex` para alinear texto e ícono.
- Los marcadores de texto (`.marker`) y los chips (`.chip`) usan `display: inline-block`.
- La alineación de la navegación y las grillas de cards (1 → 2 → 3 columnas) se resuelven con utilidades `flex` y `grid` de Tailwind directamente en el HTML.

**Pseudoclases y estados de los vínculos**

Los enlaces de navegación y los botones ("stickers") tienen estilos para `:hover` que cambian su apariencia al pasar el cursor. Como los vínculos no heredan el color del texto global, sus estados se definen explícitamente en el CSS.

**Transiciones y transformaciones**

Se usaron la propiedad `transition` y `transform` (no hay `@keyframes` en el CSS) para:
- El movimiento sutil de los "stickers" al hacer hover (`transform: rotate` + `translateY`) con una `transition` suave.
- El cambio de la sombra de los botones al pasar el cursor.
- Las variaciones de ángulo (`transform: rotate`) que diferencian visualmente cada card, post-it y polaroid (clases `.tilt-l`, `.tilt-r`, `.rotate-l`, `.rotate-r`).

**Diseño responsive**

El comportamiento responsive del layout se resuelve principalmente con los **breakpoints de Tailwind** (`md:`, `lg:`) aplicados como utilidades en el HTML, con enfoque mobile first: el layout base es de una sola columna y se amplía en pantallas más grandes.

Ejemplos concretos (Tailwind):
- El título del hero es de `text-5xl` en mobile y crece a `text-[112px]` en pantallas medianas y grandes (`md:`).
- La grilla de competencias pasa de 1 columna → 2 (`md:`) → 3 (`lg:`) según el tamaño de pantalla.
- El bloque hero pasa de layout vertical en mobile a dos columnas en pantallas más grandes.

El `styles/styles.css` aporta sólo unas pocas **media queries propias** (`@media (max-width: 768px)`): acercan la línea de margen roja al borde y ocultan la columna de perforaciones (`.holes`) en pantallas chicas, donde el contenido ocupa todo el ancho.

---

### 4.6 UX/UI y heurísticas de Nielsen

**Público objetivo**

El sitio está dirigido a la profesora de la materia, compañeras del equipo de Nexo Studio y potenciales colaboradores que buscan un perfil de desarrolladora front-end. Las decisiones de diseño (tono informal pero profesional, énfasis en competencias técnicas) responden a ese perfil.

**Heurísticas de Nielsen aplicadas:**

1. **Visibilidad del estado del sistema:** el link de la página activa en el menú tiene la clase `active` que lo diferencia visualmente, indicando al usuario en qué página está.

2. **Relación entre el sistema y el mundo real:** la estética del cuaderno escolar es un referente cultural inmediatamente reconocible. El uso de post-its, polaroids y marcadores de texto remite a objetos del mundo real, reduciendo la curva de comprensión del sitio.

3. **Control y libertad del usuario:** el menú de navegación está visible en la parte superior de todas las páginas, permitiendo moverse libremente entre secciones en cualquier momento.

4. **Consistencia y estándares:** la misma estética, los mismos colores y la misma tipografía se mantienen en las tres páginas. Los botones ("stickers") tienen el mismo estilo en todo el sitio.

5. **Prevención de errores:** el contacto se resuelve con enlaces `mailto:` directos en lugar de un formulario, lo que elimina la posibilidad de errores de validación o de envíos incompletos; el usuario escribe desde su propio cliente de correo.

6. **Reconocimiento en lugar de recuerdo:** la navegación siempre visible y el logo "MRPV." en todas las páginas orientan al usuario constantemente, sin que tenga que recordar la estructura del sitio.

7. **Estética y diseño minimalista:** a pesar de la estética decorativa del cuaderno, cada sección presenta una sola idea principal. Se usa espacio en blanco (`padding` generoso entre secciones) para que el contenido respire y no se sienta sobrecargado de información.

8. **Ayudar a reconocer y recuperarse de errores:** los enlaces de contacto indican con claridad su acción ("enviar correo", "agendar charla") y el correo se muestra de forma legible, orientando al usuario sobre qué va a pasar antes de hacer clic.

**Call to Action (CTA)**

Cada página termina con un CTA claro: el inicio y la de intereses llevan al contacto. Esto guía al usuario hacia una acción concreta en lugar de dejarlo sin un próximo paso.

**Coherencia visual**

El header, footer y sistema de estilos son idénticos en las tres páginas. Esta consistencia es fundamental en UX porque reduce la carga cognitiva del usuario y refuerza la identidad del sitio.

---

MRPV · Diseño y Desarrollo Web · UADE 2026
