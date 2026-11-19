# Little Moments Web

A mobile-first daily vlog recorder for a private, browser-local story. No account or backend is used.

## Run locally

Serve this directory over HTTPS or `localhost` (camera access requires a secure context), then open `index.html` in a current mobile browser.

## GitHub Pages

The included workflow publishes the root folder to GitHub Pages on every push to `main`. In the repository settings, enable Pages with **GitHub Actions** as the source if it is not enabled automatically.

## Notes

- Camera and microphone access are requested only after the visitor taps **เปิดกล้อง**.
- Clips and their text metadata stay in that browser's IndexedDB; they are not sent to GitHub or a server.
- Each visitor has their own local clips. Sharing the site shares the app, not the recorded videos.
- Export uses MP4 when the browser supports it, otherwise WebM. Supported formats depend on the device/browser.
