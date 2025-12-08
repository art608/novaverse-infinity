
NovaVerse Infinity — Evolution v4
================================

What's included:
- index.html           (Advanced NASA-style UI with clustering, filters, TTS)
- data_large.json      (2,000 generated objects; some have curated images)
- images/              (50 curated placeholder images, ready to show)
- download_nasa_images.sh (helper placeholder script)
- README.md            (this file)

How to host on GitHub Pages:
1. Create a new GitHub repo.
2. Upload index.html, data_large.json, images/ and other files to the repo root.
3. In repo Settings -> Pages, choose the main branch and root as the source.
4. Wait a few minutes and visit https://<username>.github.io/<repo>/

Notes:
- The UI uses browser SpeechSynthesis for audio. No server needed.
- To add real NASA images, run your own download script locally using the provided image queries or NASA Images API.
- If you want me to produce a version with <100 curated real NASA images embedded (public domain), say 'Embed NASA images' and I will prepare a zip with placeholder filenames you can replace, or attempt to fetch them if you provide URLs.
