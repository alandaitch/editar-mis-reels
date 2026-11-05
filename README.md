# Editar mis reels: template de skill para Claude Code

Este skill edita reels verticales desde la grabación cruda. Aprende tu gusto con cada corrección.

Este template no trae gustos de nadie. Claude te entrevista y lo completa con los tuyos.

## La forma más fácil

Entrá a la [página de instalación](https://alandaitch.github.io/editar-mis-reels/), copiá el mensaje y pegáselo a Claude Code.

También podés pegarle esto:

> Instalá el skill de https://github.com/alandaitch/editar-mis-reels: copiá la carpeta `editar-mis-reels` a `~/.claude/skills/` y decime qué programas faltan.

## Qué necesitás

- Claude Code.
- ffmpeg y whisper.cpp. Son gratis. Claude te ayuda a instalarlos.
- Un modelo de whisper. Pesa unos 1,6 GB.
- Node y Playwright, solo para animaciones.

Los scripts se probaron en una Mac, con grabaciones de prueba. En otro sistema, pedile a Claude que adapte los comandos.

## Cómo se usa

1. Copiá la carpeta `editar-mis-reels` de este repositorio a `~/.claude/skills/`.
2. Abrí Claude Code y escribí: `configurá mi skill de edición`.
3. Respondé la entrevista. Podés cortarla y retomarla.
4. Escribí: `editá este reel: <ruta de tu grabación>`.
5. Marcá lo que no te guste y escribí esta frase:

   > Corregilo y modificá el skill para que no lo vuelva a hacer.

La primera versión va a tener errores. Cada error se vuelve una regla.

## Qué hay en la carpeta

| Archivo | Para qué sirve |
|---|---|
| `editar-mis-reels/SKILL.md` | El flujo de edición |
| `preferencias.md` | Tu gusto. Claude lo completa con la entrevista |
| `estilo.json` | Los valores exactos de tus subtítulos |
| `correcciones.md` | Las reglas que nacen de tus correcciones |
| `references/configurar.md` | El guion de la entrevista |
| `references/medir-referencia.md` | Cómo medir un video que te gusta |
| `references/lecciones.md` | Errores comunes de edición |
| `scripts/` | Cortes, transcripción, subtítulos, armado y revisión |
| `assets/animacion-ejemplo.html` | Punto de partida para animaciones |

## Material de terceros

Usá solo material con permiso. El skill pregunta antes de usar material ajeno, salvo que definas otra regla.
