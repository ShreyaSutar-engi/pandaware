# PandaWare

An open-source, EMG-controlled prosthetic hand — built to be affordable,
understandable, and yours to customize.

📖 **Docs:** https://ShreyaSutar-engi.github.io/pandaware/

## Repository layout

```
.
├── docs/                   # MkDocs site content (Material theme)
│   ├── index.md            # Custom hero landing page (site home)
│   ├── stylesheets/extra.css
│   ├── build-it/           # Build It section
│   ├── understand-it/      # Understand It section
│   ├── model-it-yourself/  # Model It Yourself section
│   └── about/               # About section
├── mkdocs.yml              # Site config, nav, theme
├── requirements.txt        # Python deps for building the docs
├── .github/workflows/deploy.yml  # Auto-deploys docs to GitHub Pages on push to main
├── LICENSE                 # MIT — firmware / source code
└── LICENSE-DOCS.md         # CC BY 4.0 — documentation & hardware designs
```

## Local development

```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```

Then open http://127.0.0.1:8000/.

## Deployment

Docs deploy automatically to GitHub Pages via GitHub Actions
(`.github/workflows/deploy.yml`) on every push to `main`. See the setup
instructions given alongside this scaffold for one-time repo settings, or
deploy manually with:

```bash
mkdocs gh-deploy --force
```

## License

- **Documentation & hardware designs** (`docs/`, CAD/STL/STEP files): [CC BY 4.0](LICENSE-DOCS.md) — share and adapt freely, with credit to PandaWare.
- **Firmware & other source code**: [MIT](LICENSE).

See [License & Attribution](docs/about/license-attribution.md) for full
details and suggested attribution text.
