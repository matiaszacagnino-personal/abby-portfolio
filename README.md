# Portfolio web de Abby — UGC Creator

Versión web del portfolio de Canva de Abigail Quiña. Sitio estático (un solo `index.html` + assets), sin dependencias ni build: se abre con doble click o se sube a cualquier hosting estático.

## Qué mejora respecto del Canva

- Los videos se reproducen en la página (en el export de Canva quedaban congelados).
- Link navegable para mandar a las marcas, en vez de un PDF pesado.
- Filtros por nicho en la galería de fotos.
- Botones directos de mail y WhatsApp.
- Corrige los typos del original ("jewerly", "CONTEN T").

## Pendientes antes de publicar

1. **Videos**: poner los .mp4 reales en `assets/videos/` con estos nombres exactos
   (por ahora se ve el poster con el botón de play atenuado si el archivo no está):
   - `moda-unboxing.mp4`, `moda-camara.mp4`, `moda-outfit.mp4`, `moda-aesthetic.mp4`
   - `belleza-camara.mp4`, `belleza-resena.mp4`, `belleza-aesthetic.mp4`, `belleza-voz.mp4`
   - `home-camara.mp4`, `home-voz.mp4`, `home-pijama.mp4`, `home-manta.mp4`
   - `jewelry-1.mp4`, `fashion-skincare.mp4`, `lifestyle-honey.mp4`, `lifestyle-colchon.mp4`

   Recomendado: exportar en 720×1280 (9:16), H.264, ~2-4 MB por video para que cargue rápido.

2. **Redes**: completar los links reales de Instagram y TikTok en el hero
   (buscar el comentario `TODO` en `index.html`).

## Deploy

Cualquiera de estas opciones sirve:

- **GitHub Pages**: crear repo, subir todo, Settings → Pages → deploy from branch.
- **Netlify / Vercel**: arrastrar la carpeta al dashboard, listo.

Si los videos pesan mucho para GitHub (límite 100 MB por archivo, repo ideal < 1 GB),
Netlify o Vercel los sirven sin drama.
