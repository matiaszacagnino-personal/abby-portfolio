# Portfolio web de Abby — UGC Creator

Versión web del portfolio de Canva de Abby (Abigail Quiña). Sitio estático (un solo `index.html` + assets), sin dependencias ni build: se abre con doble click o se sube a cualquier hosting estático.

El portfolio mantiene la estética glamour (crema, serif Italiana, terracota) y tiene una **sección Tech & Apps** (`#tech`) que cambia de clima: fondo oscuro, Space Grotesk + IBM Plex Mono, acento ámbar. Vende el perfil developer de Abby (Baufest/Oracle, según su CV) como credibilidad para reviews de apps de fintech, delivery, fitness y gadgets.

## Qué mejora respecto del Canva

- Los videos se reproducen en la página (en el export de Canva quedaban congelados).
- Link navegable para mandar a las marcas, en vez de un PDF pesado.
- Filtros por nicho en la galería de fotos.
- Botones directos de mail y WhatsApp.
- Corrige los typos del original ("jewerly", "CONTEN T").

## Videos

Los 15 videos reales viven en `assets/videos/` (720×1280 9:16, H.264 CRF 27 a 30 fps, audio
AAC 96k, `+faststart`), convertidos con ffmpeg desde los .MOV originales que están en
`Desktop/Abby Project/Portfolio/Videos/`. Cada poster de `assets/posters/` es un frame del
propio video, así el preview siempre coincide con lo que se reproduce.

13 videos son de los nichos UGC (moda ×4, belleza ×3, home ×2, joyería, skincare, gastronomía
y estética) y 2 son de la sección Tech: `tech-ia.mp4` (review de ChatGPT con screen recording)
y `tech-luz.mp4` (unboxing de una luz LED para sets). Los mockups de Fintech y Delivery de la
sección Tech siguen como placeholders "Próximamente".

## Deploy

Cualquiera de estas opciones sirve:

- **GitHub Pages**: crear repo, subir todo, Settings → Pages → deploy from branch.
- **Netlify / Vercel**: arrastrar la carpeta al dashboard, listo.

Si los videos pesan mucho para GitHub (límite 100 MB por archivo, repo ideal < 1 GB),
Netlify o Vercel los sirven sin drama.
