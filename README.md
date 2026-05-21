# Portfolio · María del Rosario Presedo Valenzuela

Rediseño en estilo cuaderno/diario - papel crema con líneas, washi tape, post-its, doodles a mano y stickers como botones.

## Stack

- HTML5 semántico
- [Tailwind CSS](https://tailwindcss.com/) (vía Play CDN)
- CSS propio en `styles.css` para los patrones de cuaderno (líneas, marcador, polaroids, etc.)
- Google Fonts: **Caveat** (manuscrita) · **Newsreader** (serif) · **JetBrains Mono** (detalles)

## Estructura

```
.
├── index.html        # Inicio · sobre mí · competencias · Nexo Studio
├── intereses.html    # Mis intereses · filosofía
├── contacto.html     # Correo · disponibilidad · Nexo Studio
├── styles.css        # Patrones de cuaderno (líneas, marker, post-its, tape, etc.)
└── img/
    └── infografia.jpg
```

## Desarrollo

Es HTML estático, no necesita build. Abrí cualquier archivo directamente en el navegador, o serví la carpeta:

```bash
npx serve .
```

## Despliegue (GitHub Pages)

Subí el contenido de esta carpeta al branch que sirvas (por ej. `main`) y activá Pages en Settings → Pages.

---

MRPV · Diseño y Desarrollo Web · UADE 2026
