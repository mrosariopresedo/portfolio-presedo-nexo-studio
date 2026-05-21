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
Formulario de contacto con campos de nombre, email y mensaje. Incluye dirección de correo directa y enlace al sitio de Nexo Studio.

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

| Color | Valor HEX | Uso |
|---|---|---|
| Crema | `#F5F0E8` | Fondo principal (el "papel") |
| Tinta oscura | `#2C2416` | Texto principal |
| Rojo margen | `#C0392B` | Logo, líneas de margen, énfasis |
| Amarillo highlight | `#FFF59D` | Resaltado tipo marcador |
| Rosa | `#FFB3C6` | Marcador alternativo |

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

**Formulario (`contacto.html`):**
- `type="email"` en el campo de correo para validación automática del formato.
- `type="text"` en el campo de nombre y `<textarea>` para el mensaje.
- `required` en todos los campos obligatorios.
- `placeholder` en cada campo para orientar al usuario.
- `<label>` asociados a cada campo con el atributo `for`.

---

### 4.5 CSS: modelo de caja, cascada y diseño responsive

**Arquitectura del CSS**

El sitio combina **Tailwind CSS** (desde CDN) para el layout y los espaciados, con el archivo `styles/styles.css` para los estilos que definen la estética del cuaderno: el patrón de líneas del fondo, los post-its, el efecto polaroid, las cintas washi tape y las animaciones de hover.

El CSS propio usa **variables CSS** (custom properties) al inicio del archivo para centralizar todos los colores y fuentes, siguiendo el principio de separación entre estructura (HTML) y presentación (CSS).

**Modelo de caja (Box Model)**

El modelo de caja está presente en todos los componentes:
- Las **cards de competencias** tienen `padding` interno para separar el contenido del borde, y un `border` que simula el borde de una nota de papel.
- Los **post-its** tienen `padding` generoso y `margin` para que no queden pegados entre sí.
- El **contenedor principal** usa `max-width` y `margin: auto` para centrarse, con `padding` lateral que aumenta en pantallas más grandes.

Al inicio del CSS se usa el **selector universal** con `* { box-sizing: border-box; }` para que el `padding` y el `border` queden incluidos dentro del ancho declarado de cada elemento, facilitando el cálculo del layout.

**Propiedad `display`**

- La navegación usa `display: flex` para alinear los ítems del menú en horizontal.
- Las grillas de cards usan `display: grid` con columnas que se adaptan: una columna en mobile, dos en tablet, tres en escritorio.
- Los elementos decorativos (perforaciones, cintas) usan `display: block` para ocupar su propio espacio sin interferir con el flujo del texto.

**Pseudoclases y estados de los vínculos**

Los enlaces de navegación y los botones ("stickers") tienen estilos para `:hover` que cambian su apariencia al pasar el cursor. Como los vínculos no heredan el color del texto global, sus estados se definen explícitamente en el CSS.

**Animaciones y transiciones**

Se usaron `@keyframes` y la propiedad `transition` para:
- Las rotaciones sutiles de las cards al hacer hover (efecto de papel que se mueve).
- El cambio de color y fondo en los botones al pasar el cursor.
- Las variaciones de ángulo (`transform: rotate`) que diferencian visualmente cada card.

**Diseño responsive (Mobile First)**

El sitio está construido con enfoque **mobile first**: el layout base es de una sola columna (para pantallas pequeñas) y se amplía mediante **media queries** (breakpoints) de Tailwind para pantallas más grandes.

Ejemplos concretos:
- El título del hero es de `64px` en mobile y crece a `112px` en pantallas grandes.
- La columna lateral del cuaderno (con las perforaciones) solo aparece en pantallas medianas y grandes; en mobile el contenido ocupa todo el ancho.
- La grilla de competencias pasa de 1 columna → 2 → 3 según el tamaño de pantalla.
- El bloque hero pasa de layout vertical en mobile a dos columnas en pantallas más grandes.

---

### 4.6 UX/UI y heurísticas de Nielsen

**Público objetivo**

El sitio está dirigido a la profesora de la materia, compañeras del equipo de Nexo Studio y potenciales colaboradores que buscan un perfil de desarrolladora front-end. Las decisiones de diseño (tono informal pero profesional, énfasis en competencias técnicas) responden a ese perfil.

**Heurísticas de Nielsen aplicadas:**

1. **Visibilidad del estado del sistema:** el link de la página activa en el menú tiene la clase `active` que lo diferencia visualmente, indicando al usuario en qué página está.

2. **Relación entre el sistema y el mundo real:** la estética del cuaderno escolar es un referente cultural inmediatamente reconocible. El uso de post-its, polaroids y marcadores de texto remite a objetos del mundo real, reduciendo la curva de comprensión del sitio.

3. **Control y libertad del usuario:** el menú de navegación está visible en la parte superior de todas las páginas, permitiendo moverse libremente entre secciones en cualquier momento.

4. **Consistencia y estándares:** la misma estética, los mismos colores y la misma tipografía se mantienen en las tres páginas. Los botones ("stickers") tienen el mismo estilo en todo el sitio.

5. **Prevención de errores:** el formulario valida los campos con `required` y `type="email"` antes de permitir el envío, evitando que el usuario mande un formulario incompleto o con un correo con formato incorrecto.

6. **Reconocimiento en lugar de recuerdo:** la navegación siempre visible y el logo "MRPV." en todas las páginas orientan al usuario constantemente, sin que tenga que recordar la estructura del sitio.

7. **Estética y diseño minimalista:** a pesar de la estética decorativa del cuaderno, cada sección presenta una sola idea principal. Se usa espacio en blanco (`padding` generoso entre secciones) para que el contenido respire y no se sienta sobrecargado de información.

8. **Ayudar a reconocer y recuperarse de errores:** los campos del formulario tienen `placeholder` que describe qué información se espera en cada uno, orientando al usuario antes de que cometa un error.

**Call to Action (CTA)**

Cada página termina con un CTA claro: el inicio y la de intereses llevan al contacto. Esto guía al usuario hacia una acción concreta en lugar de dejarlo sin un próximo paso.

**Coherencia visual**

El header, footer y sistema de estilos son idénticos en las tres páginas. Esta consistencia es fundamental en UX porque reduce la carga cognitiva del usuario y refuerza la identidad del sitio.

---

MRPV · Diseño y Desarrollo Web · UADE 2026
