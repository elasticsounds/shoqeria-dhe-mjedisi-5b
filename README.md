# Shoqëria dhe mjedisi — 5B

Accessible digital textbook reader with Albanian and English interfaces, read aloud, Easy Read, glossary, interactive activities, and sign-language video controls.

Read the book: https://elasticsounds.github.io/shoqeria-dhe-mjedisi-5b/

The reader has 39 screens, including 25 activity screens. Eight supplied sign-language clips repeat in numbered order across the 33 screens from `pg008_sec001` onward.

## Run locally

From this directory:

```sh
python3 -m http.server 8766 --bind 127.0.0.1
```

Then open http://127.0.0.1:8766/ . The bundled offline preloader also supports opening `index.html` directly.

## GitHub Pages

Publish from the `main` branch and the repository root (`/`). The `.nojekyll` file lets Pages serve the reader as ordinary static files. No build step is needed.

Changes to files embedded in `assets/offline-preloader.js` must also be reflected in that generated file so navigation and offline behavior remain consistent.
