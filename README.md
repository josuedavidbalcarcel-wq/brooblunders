# BrooBlunders (versión alojada)

Proyecto estático: `index.html` + carpeta `engine/`. No hay servidor ni compilación.

## Publicar (gratis, ~2 min)
- **Netlify:** entra en app.netlify.com/drop y arrastra esta carpeta. Te da un enlace para compartir.
- **GitHub Pages:** sube los archivos a un repositorio → Settings → Pages → rama `main`.

## Stockfish 16 (más fuerte y rápido)
1. Descarga el paquete npm `stockfish` versión 16 (`npm i stockfish@16`).
2. Copia a `engine/` los archivos `stockfish-nnue-16-single.js` y su `.wasm` (mismo nombre base).
3. Sin esos archivos la página usa Stockfish 10 desde un CDN, que funciona pero es más débil.
(No pude probar esta carga desde aquí: si el motor no aparece como "Stockfish 16" en Análisis, dímelo.)

## Profesor
Fuera de claude.ai necesita una API key de Anthropic (console.anthropic.com). Cada persona pone la suya la primera vez; se guarda solo en su navegador. Tiene coste por uso.

## Editar
Todo está en `index.html` (HTML + CSS + JS). Edítalo con cualquier editor, o súbemelo a Claude y pídele cambios; después vuelve a publicar.
Los datos (partidas, revisiones) viven en el navegador de cada persona.
