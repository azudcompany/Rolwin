# Rolwin Riegos — rediseño (vista previa)

Página única estática para mostrar la propuesta de rediseño de la web de Rolwin Riegos (Luján de Cuyo, Mendoza).
No necesita compilación: todo está en `public/` (`index.html`, `media/`, `video/`).

## Publicar en Cloudflare

El proyecto está conectado como **Worker con archivos estáticos** (Workers Builds): cada push a `main` se publica solo.
`wrangler.jsonc` le indica a Cloudflare que sirva la carpeta `public/` (no hace falta comando de compilación;
el comando de publicación es el predeterminado, `npx wrangler deploy`).

La vista previa está marcada `noindex` (no aparece en Google). Para publicarla como web definitiva hay que sacar
la línea `noindex` de `public/index.html` y de `public/_headers`.

## Contenido

- `video/journey-*.mp4` (H.264, todos los cuadros completos) y `*.webm` (respaldo): el recorrido del agua que avanza con el scroll.
  Generados con Higgsfield (Kling) e ilustrativos.
- `media/`: fotos (ilustrativas salvo la camioneta de Rolwin), logos y la fuente Onest (SIL OFL, ver `media/onest-OFL.txt`).
- El formulario de consulta no envía datos a ningún servidor: arma el mensaje y abre WhatsApp.
