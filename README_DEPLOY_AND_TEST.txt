APDS Mobile Survey V0.9.6.5 — HTTPS-READY TEST PACKAGE

IMPORTANT: This package is prepared for HTTPS hosting; it has NOT been deployed to a live URL.

DEPLOYMENT OPTION: GitHub Pages
1. Create a separate repository for this trial (do not deploy the private pricing manager source). Upload index.html, manifest.webmanifest, service-worker.js to repository root.
2. Repository Settings > Pages > Build and deployment > Deploy from a branch > main / root > Save.
3. Open the HTTPS address shown by GitHub Pages in Chrome on both devices. Do not open the downloaded HTML file.
4. Be aware: GitHub Pages sites are publicly reachable on standard plans even when source repository visibility differs. Do NOT publish proprietary source, client details, photos or real customer data. This is a dummy-data trial only. Hosting static files does not itself upload survey records, but browser and service risks remain.
5. On each device allow Camera and Microphone permissions when requested. Select Video & voice assisted and press Start camera preview, then Start recording. Live speech is a separate Start live speech action and may fail due to browser/service support.
6. Download video before closing the page; save equipment record and export JSON. Media files are NOT embedded in JSON. The service worker caches only the app shell, NOT video recordings or survey exports.
7. A network connection is required for the first load. Cached shell may open offline after first visit, but camera, speech and storage availability vary; speech often requires network. This is not production-grade offline storage.
8. Existing local-file survey data will NOT automatically appear at the new HTTPS origin. Export the old JSON first. There is no JSON re-import feature in this version.
9. Test camera and speech separately before attempting simultaneous operation. Chrome may not support concurrent recognition and MediaRecorder reliably.
10. Do not use for real customer surveys until secure authentication, persistent media storage, encryption and backup/recovery are implemented.

TROUBLESHOOTING
- Page shows Secure context NO: use the HTTPS site address, not file:// or content://.
- Camera NotAllowedError: Chrome site settings / Android permissions; allow camera and microphone.
- Camera NotFoundError: camera missing or unavailable.
- Camera NotReadableError: close other apps using camera.
- Speech recognition API detected but fails: browser service/network may be unavailable; use video and later review.
- Phone/tablet local storage is independent. Keep exports separate.
