# Estudio Jurídico INA — sitio web

## Regla principal
Desde 2026-11-03 la fuente de verdad es **este repositorio**, carpeta `sitio/`.
Los Artifacts de claude.ai quedan como historial: NO se editan ni se republican, y pueden estar desactualizados.
Todos los cambios se hacen en `sitio/` y se suben a este repo (commit + push a `main`).

## Estructura de `sitio/`
- `sitio/index.html` es la home (URL: estudioina.com.ar). Sus imágenes están en `sitio/`.
- Cada otra página vive en su carpeta: `sitio/<página>/index.html` + sus imágenes. La carpeta define la URL (importa para SEO: no renombrar sin avisar).
- Enlaces entre páginas: SIEMPRE relativos (`../penal/`, `../#contacto`; desde la home `penal/`). Nunca a claude.ai/artifact.
- WordPress, si se mantiene, va en una carpeta interna que el desarrollador (Gustavo) agrega al `.gitignore`. No tocar esa carpeta.
- Los enlaces de Prensa escrita a `estudioina.com.ar/<nota>/` apuntan a WordPress; actualizarlos cuando Gustavo pase las URLs nuevas.

## Cómo hacer cualquier cambio
1. Editar el HTML directamente en `sitio/`.
2. Si el cambio toca el menú, el footer o los datos de contacto, aplicarlo en TODAS las páginas de la tabla.
3. Verificar que no queden enlaces rotos (hrefs, imágenes, anchors) antes de subir.
4. Commit y push a `main`. Confirmar a Deborah qué se subió.

## Páginas
| Página | Ruta |
|---|---|
| Home | `sitio/index.html` |
| Derecho Penal | `sitio/penal/` |
| Migratorio Argentino | `sitio/migratorio-argentino/` |
| Sobre nosotros | `sitio/sobre-nosotros/` |
| Prensa escrita | `sitio/prensa-escrita/` |
| Prensa audiovisual | `sitio/prensa-audiovisual/` |
| Contacto | `sitio/contacto/` |
| Política de privacidad | `sitio/politica-de-privacidad/` |
| Juicio oral, Migratorio EEUU | (pendiente: crear página) |

## Estilo / contenido
- Español rioplatense (es-AR). Sin promesas de resultado ("garantizamos", "ganamos") por políticas de Google Ads.
- Imágenes: usar el skill `insertar-imagen-web`.

## Pendientes conocidos
- La imagen de fondo del encabezado de Migratorio (`control-migratorio-aeropuerto-argentinos-1167.webp`) mide solo 644 px de ancho; si se ve pixelada, reemplazar por una de al menos 1600 px.

## _archivo-prototipos/
Borradores viejos. Solo referencia; no editar ni publicar desde ahí.
