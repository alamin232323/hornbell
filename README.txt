HORNBELL PWA (MVP) — upload this whole folder as a website.

Files: index.html (the app), manifest.webmanifest, sw.js (offline cache), icons.

Free static hosting options (check each service's current free terms before relying on it):
  GitHub Pages, Cloudflare Pages, Netlify, Vercel.
It must be served over HTTPS (or localhost) for install and offline to work.
Opening index.html straight from a file does NOT enable install or offline.

Test locally:  python3 -m http.server 8080   then open http://localhost:8080

Android Chrome: menu > Install app. iPhone Safari: Share > Add to Home Screen.

Updating: change index.html, then bump V in sw.js ("hornbell-v2") so phones refresh the cache.

Limits (honest): this is a PWA, not a native app. iOS may clear storage of rarely used web apps;
data is on-device only until a backend is added. Push notifications are not included yet.
