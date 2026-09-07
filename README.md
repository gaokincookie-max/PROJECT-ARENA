# PROJECT ARENA

GitHub Pages-ready browser prototype.

## Repository structure

```text
/
├─ index.html
├─ assets/
│  ├─ blade_face.png
│  ├─ blade_unit.png
│  ├─ blade_symbol.png
│  └─ blade_intercept.png
├─ README.md
└─ .gitignore
```

## GitHub Pages publishing

1. Create a GitHub repository.
2. Put `index.html`, `assets/`, `README.md`, and `.gitignore` at the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select `main` and `/ (root)`.
6. Save.

The game will be served from the repository's GitHub Pages URL.

## Local test

You can open `index.html` directly, or run:

```bash
python -m http.server 8000
```

and open `http://localhost:8000`.

## Asset policy

Keep future character portraits, board sprites, symbols, and cut-ins in `assets/`.
Avoid embedding large images as Base64 in `index.html`; this keeps the page lightweight and easier to maintain.
