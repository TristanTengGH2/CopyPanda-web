# CopyPanda web app

A cozy red-panda study timer with a cafe scene, local notes, a study calendar,
goals, leaves, and optional bookmarks for your next session.

The Windows Godot overlay is maintained separately in the original
[CopyPanda repository](https://github.com/TristanTengGH2/CopyPanda).
This repository hosts the browser app with GitHub Pages.

## Run locally

Node.js 18 or later is sufficient. No packages or API key are required.

```sh
npm start
npm test
```

Open `http://127.0.0.1:4173/`. The static site is the `web/` directory.

## Hosting

GitHub Pages deploys `web/` through `.github/workflows/pages.yml` on pushes to
`main`. Repository Settings > Pages must use **GitHub Actions** as the source.
The expected project URL is `https://tristantenggh2.github.io/CopyPanda-web/`.

Progress is stored in browser local storage for the hosting origin. Switching
from localhost to the hosted site does not transfer your existing progress.
Native overlay progress is also separate. Clearing site data removes progress.
Together now connects real guest rooms across the website and Windows overlay.
Share expiring QR/link/code invitations, keep independent timers, or opt into
a shared start. QR generation and scanning run locally; no GPS is collected.
Email sign-in and cross-device leaves/history remain disabled pending sender setup.
See [the network spec](NETWORK_SPEC.md) and [backend setup](https://github.com/TristanTengGH2/CopyPanda/blob/main/backend/README.md).

See `SPEC.md` for product direction and `web/assets/ASSETS.md` for artwork provenance.
