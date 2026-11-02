# Bhagavad Gita – Universal Wisdom (PWA)

A responsive, installable Progressive Web App reader for Android and web.

## Run
Upload this folder to any static HTTPS host (GitHub Pages, Netlify, Cloudflare Pages, etc.) or serve it locally using a static web server. Service workers/PWA installation require HTTPS or localhost; opening `index.html` directly as a `file://` URL will not enable offline/PWA features.

## Features implemented
- All 18 chapters and traditional verse counts (700 total).
- Live verse retrieval from the Vedic Scriptures API (`https://vedicscriptures.github.io`).
- Sanskrit original and IAST transliteration.
- English and Hindi translation/commentary fields where the API provides them.
- Selectable named commentary sources.
- Chapter/verse navigation, verse reference search, loaded/offline keyword search.
- Local bookmarks, light/dark mode, adjustable font size.
- Browser text-to-speech, share/copy, per-chapter offline caching.
- PWA manifest and service worker; Android install prompt when browser supports it.
- No paid API key required by this client.

## Data source and rights
The app uses the public Vedic Scriptures Bhagavad Gita API. Its API repository is at https://github.com/vedicscriptures/bhagavad-gita-api and identifies its software license as GPL-3.0. The static API documentation is at https://github.com/vedicscriptures/vedicscriptures.github.io. The underlying API includes verse text, transliteration, and named commentator/translation fields. Check the source's current terms and the rights for individual translations/commentaries before commercial use or redistribution. Attribution is included in the app.

## Language scope
This build exposes English, Hindi and Sanskrit. It does not claim that all languages are already verified. Marathi and additional world languages need reviewed translation datasets and rights/attribution checks; this app deliberately does not invent or machine-label those translations as verified.

## Production caveats
This is a working client-side application, not a hosted public deployment or a signed Android APK. The scripture API is a third-party dependency. Offline use is limited to the app shell and content previously fetched/cached. Bookmarks are local to one browser/device; there is no cloud account sync. For Play Store release, wrap the hosted PWA or build a native Android package, test on target devices, provide a privacy policy, and complete store review.
