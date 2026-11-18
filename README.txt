Vocabulary Studio — offline-ready app

Files:
- index.html: all three modes; CSS and JavaScript are embedded
- manifest.json: web app manifest
- service-worker.js: caches the app and word book
- words.json: static Chinese-English word book

Setup and offline test:
1. Keep all files together in one folder.
2. Run the folder from localhost or HTTPS (for example, VS Code Live Server).
3. Open the page once while online and wait for the service worker to install.
4. Refresh once.
5. In DevTools, enable Network > Offline and refresh again.
6. The page, word book, and review queue should remain available.

Important: Service Workers do not work from file:// URLs. Use localhost or HTTPS.
No accounts, sync, or background word updates are included.
