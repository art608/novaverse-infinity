
NovaVerse Infinity — Massive Pack
================================

Contents:
- index.html (NASA-style UI with search, zoom and TTS)
- data_large.json (5,000 auto-generated objects)
- download_nasa_images.sh (script generator inside the UI to fetch images using NASA Images API)
- README.md (this file)

How to use:
1. Unzip and review files locally.
2. To host on GitHub Pages:
   - Create a new GitHub repo.
   - Upload index.html and data_large.json to the repo root (or gh-pages branch).
   - Go to repository Settings -> Pages and select the branch to publish.
   - Your site will be available at https://<username>.github.io/<repo>/

Image download:
- The UI can generate a shell script (download_nasa_images.sh) that uses the NASA Images API and 'jq' to fetch images.
- You need 'curl' and 'jq' installed. Run: bash download_nasa_images.sh
- For high-volume image downloads, use NASA API responsibly; they have rate limits and usage terms.

Audio:
- The site uses the browser's SpeechSynthesis API to play audio descriptions (no server required).

Performance:
- The map renders thousands of SVG nodes — for mobile or weak devices, consider server-side tiling or progressive clustering.
- To expand to tens/hundreds of thousands, convert the renderer to WebGL (e.g., using PixiJS or regl) for better performance.
