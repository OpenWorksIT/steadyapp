# steadyapp.co.za

The website for [Steady](https://github.com/OpenWorksIT/steady), check-ins between therapy sessions.

- **Science and research:** Kempie van Rooyen and VR Clinical Psychology.
- **Code and development:** OpenWorks IT.

A [Hugo](https://gohugo.io) site with its own templates (no theme), no JavaScript, no trackers. Hosted on GitHub Pages: `.github/workflows/pages.yml` builds and publishes every push to `main`.

## Editing

| What | Where |
|---|---|
| Page text | `content/*.md` (the home page is `layouts/home.html`) |
| Menu, contact details, store links | `hugo.toml` |
| Look | `assets/css/site.css` |
| The home page's fortnight line | `tools/fortnight.py` (writes `layouts/_partials/fortnight.html`) |
| App screenshots | `static/img/screens/` (fictional practice and patients only) |

The store links are in `hugo.toml` (`appStore`, `googlePlay`); the patients page shows a button for each. What the site says about Steady follows the Steady repository's README and docs (`docs/VERSIONS.md` has what changed in each version): check the pages against them after a release that changes what practices, patients or the community see.

The privacy policy stays at [openworks.co.za/steady/privacy](https://www.openworks.co.za/steady/privacy/), which the app stores link to.

## Running it locally

```bash
hugo server     # http://localhost:1313
```

Needs Hugo 0.146 or newer (extended not required). The workflow pins the version it builds with (`HUGO_VERSION`).

## Licence

Code: GNU AGPL v3 or later, like Steady. Fonts: Atkinson Hyperlegible Next and Barlow, SIL Open Font License (`static/fonts/`).
