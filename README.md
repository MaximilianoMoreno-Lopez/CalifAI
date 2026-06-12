# CALIFAI — Web corporativa

Sitio web estático de **CALIFAI CONSULTING, S.L.U.** — consultora boutique (Córdoba)
que une economía aplicada, IA / automatización y sostenibilidad.

Construido en HTML + CSS + JS mínimo, sin build. Listo para **GitHub Pages**.

## Estructura

```
index.html          One-page con secciones ancladas (hero, servicios, por qué,
                    proceso, nosotros, sectores, contacto).
aviso-legal.html    Plantilla de aviso legal (LSSI).
privacidad.html     Plantilla de política de privacidad (RGPD / LOPDGDD).
styles.css          Estilos (variables de marca, responsive mobile-first).
script.js           Menú móvil + año dinámico del footer.
assets/             Logos SVG de la marca.
.nojekyll           Evita el procesado Jekyll en GitHub Pages.
```

## Publicar en GitHub Pages

1. Sube el repo a GitHub.
2. **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*,
   Branch = `main`, carpeta = `/ (root)`.
3. La web quedará en `https://<usuario>.github.io/<repo>/`.

No hay paso de build: el `index.html` está en la raíz.

## Pendientes (placeholders que solo sabes tú)

Busca el texto `[pendiente]` / `(pendiente)` y rellena:

- **Contacto:** email real, teléfono, URL de LinkedIn.
- **Formulario:** en `index.html`, reemplaza el `action="mailto:..."` por tu
  endpoint de [Formspree](https://formspree.io) o [Getform](https://getform.io)
  (`<form action="https://formspree.io/f/XXXX" method="POST">`).
- **CIF** de la S.L.U. (footer y páginas legales).
- **Páginas legales:** completa los datos registrales y revísalas con un profesional.
- **Casos de éxito / testimonios:** añádelos en la sección «Sectores» cuando los tengas.

## Favicon en varios formatos (opcional)

El favicon usa `assets/califai_icono_metalico.svg` (soportado por navegadores modernos).
Si quieres `.png 512px` e `.ico` para máxima compatibilidad, exporta ese SVG, p. ej.:

```bash
# requiere rsvg-convert o inkscape
rsvg-convert -w 512 -h 512 assets/califai_icono_metalico.svg -o assets/favicon-512.png
```

## Marca

| Uso | Hex |
|---|---|
| Azul marino | `#1B2A8E` |
| Oro | `#F6C61C` |
| Naranja (acento) | `#E07B1E` |
| Azul medianoche | `#0A1020` → `#16203A` |
| Crema | `#F6F2E9` |

Tipografías: **Fraunces** (titulares) + **Inter** (texto), vía Google Fonts.
