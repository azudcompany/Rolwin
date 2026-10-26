# Rolwin Riegos — rediseño (vista previa)

Página única estática para mostrar la propuesta de rediseño de la web de Rolwin Riegos (Luján de Cuyo, Mendoza).
No necesita compilación: `index.html` + `media/` + `video/`.

## Publicar en Cloudflare Pages

1. Cloudflare → Workers & Pages → Create → Pages → Connect to Git → elegir este repositorio.
2. Framework preset: **None**. Build command: *(vacío)*. Build output directory: **/**.
3. Deploy. Cada push a `main` vuelve a publicar.

La vista previa está marcada `noindex` (no aparece en Google). Para publicarla como web definitiva hay que sacar
la línea `noindex` de `index.html` y de `_headers`.

## Contenido

- `video/journey-*.mp4` (H.264, todos los cuadros completos) y `*.webm` (respaldo): el recorrido del agua que avanza con el scroll.
  Generados con Higgsfield (Kling) e ilustrativos.
- `media/`: fotos (ilustrativas salvo la camioneta de Rolwin), logos y la fuente Onest (SIL OFL, ver `media/onest-OFL.txt`).
- El formulario de consulta no envía datos a ningún servidor: arma el mensaje y abre WhatsApp.
