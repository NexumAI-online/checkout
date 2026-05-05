# Nexum Academy Pro™ — Checkout Landing

Landing page de checkout para **Nexum Academy Pro™** — programa de 90 días para construir una agencia de IA.

## Stack

- HTML + CSS + JavaScript vanilla, single-file
- Inter (Google Fonts) + JetBrains Mono
- Lucide icons (CDN)
- Sin frameworks, sin build step

## Estructura

```
.
├── index.html              # Landing completa
└── assets/
    ├── favicon.svg         # Favicon oficial Nexum
    ├── logo-nexum-ai.svg   # Logo oficial (usado en navbar y footer)
    ├── logo-nexum-ai.png
    ├── founder-jp.png      # Retrato Juan
    └── founder-agus.png    # Retrato Agus
```

## Deploy

Cualquier hosting estático funciona (Vercel, Netlify, Cloudflare Pages, GitHub Pages). No requiere build.

## Configuración

Editar el bloque `CONFIG` dentro del `<script>` en `index.html`:

```js
const CONFIG = {
  STRIPE_CHECKOUT_URL: 'https://buy.stripe.com/...',
  DEADLINE_DATE: new Date('2026-05-10T23:59:59-03:00'),
  PRICE_FOUNDERS: 1500,
  PRICE_REGULAR: 2000,
  ...
};
```

Reemplazar `STRIPE_CHECKOUT_URL` con el link real de Stripe Payment Link cuando esté listo.
