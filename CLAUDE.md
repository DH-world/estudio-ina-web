# Estudio Jurídico INA — sitio web

## Regla principal
El sitio de INA vive en **Artifacts de claude.ai**. El Artifact publicado es la ÚNICA fuente de verdad.
Los archivos .html locales NO son el sitio: si edito uno, el sitio no cambia.

## Carpeta `sitio/` (espejo en Git)
`sitio/<página>/index.html` + imágenes es una COPIA de cada Artifact, bajada el 2026-10-13 para tener historial en Git.
Sentido único: **Artifact → carpeta**. Nunca editar `sitio/` a mano esperando que cambie la web.
Después de publicar un cambio en un Artifact, actualizar la copia (leer el Artifact con `path`) y hacer un commit.
Si un archivo de `sitio/` difiere del Artifact, gana el Artifact.

## Cómo hacer cualquier cambio
1. Leer el Artifact actual con `Artifact action:"read"` y la URL de la tabla de abajo (nunca partir de memoria ni de un .html viejo).
2. Escribir el HTML modificado en el scratchpad (carpeta temporal), NO en Downloads ni en el Escritorio.
3. Republicar con `Artifact` pasando `url:` de la página (así se actualiza el mismo link; sin `url` se crea uno nuevo y se rompe el menú).
4. Confirmar al usuario con el link. Si no se publicó, decirlo.
- Nunca crear archivos .html en Downloads.
- Si el cambio toca el menú, el footer o los datos de contacto, hay que aplicarlo en TODAS las páginas de la tabla.

## Páginas (Artifact = fuente)
| Página | URL |
|---|---|
| Home | https://claude.ai/artifact/WQEQKzrdroQFUnxqcTZnap |
| Derecho Penal | https://claude.ai/artifact/RgbfvGP2fbWSH9vMsFHxik |
| Migratorio Argentino | https://claude.ai/artifact/8RC1Jgt3n6tC5d3a9FwgM2 |
| Sobre nosotros | https://claude.ai/artifact/STnBMJ6PBT6D6e2eNiujvw |
| Prensa escrita | https://claude.ai/artifact/WzJ2BH9nsdRgjf27m9KsQ7 |
| Prensa audiovisual | https://claude.ai/artifact/TCuNnbEd3t199d7sKXHZSU |
| Contacto | https://claude.ai/artifact/L6DuxAPyjeozPcwwr8PY62 |
| Juicio oral, Migratorio EEUU, Política de privacidad | (pendiente: completar URL) |

## Estilo / contenido
- Español rioplatense (es-AR). Sin promesas de resultado ("garantizamos", "ganamos") por políticas de Google Ads.
- Imágenes: usar el skill `insertar-imagen-web`.

## _archivo-prototipos/
Borradores viejos movidos desde Downloads. Solo referencia; no editar ni publicar desde ahí.
