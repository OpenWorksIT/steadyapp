# steadyapp.co.za

The website for [Steady](https://github.com/OpenWorksIT/steady), check-ins between therapy sessions.

- **Science and research:** Kempie van Rooyen and VR Clinical Psychology.
- **Code and development:** OpenWorks IT.

A [Hugo](https://gohugo.io) site with its own templates (no theme), no JavaScript, no trackers. Hosted on GitHub Pages: `.github/workflows/pages.yml` builds and publishes every push to `main`.

## Editing

| What | Where |
|---|---|
| Page text | `content/*.md` (the home page is `layouts/home.html`) |
| Papers | `content/papers/` (see "Publishing a paper") |
| Menu, contact details, store links | `hugo.toml` |
| Look | `assets/css/site.css` |
| The home page's fortnight line | `tools/fortnight.py` (writes `layouts/_partials/fortnight.html`) |
| App screenshots | `static/img/screens/` (fictional practice and patients only) |

The store links are in `hugo.toml` (`appStore`, `googlePlay`); the patients page shows a button for each. What the site says about Steady follows the Steady repository's README and docs (`docs/VERSIONS.md` has what changed in each version): check the pages against them after a release that changes what practices, patients or the community see.

The privacy policy stays at [openworks.co.za/steady/privacy](https://www.openworks.co.za/steady/privacy/), which the app stores link to.

## Publishing a paper

Papers from the Steady Community go on `/papers/` (`content/papers/`, templates in `layouts/papers/`), each with a DOI from Zenodo. OpenWorks IT runs the Steady community on Zenodo (`zenodo.org/communities/steadyapp`: make it once, as OpenWorks, with the description and curation policy from `content/papers/_index.md`; if the name is taken, note the one used here); authors deposit with their own Zenodo account and ORCID, and OpenWorks accepts the record into the community. Licence: CC BY 4.0, always.

1. **Ready to publish?** The paper has been open for comment in the forum (Research and studies) for at least two weeks, and the author says, in writing, that it's ready and may go out under CC BY 4.0.
2. **Check it:** every reference and link leads to what it's cited for; no patient can be identified; a study with patients' data names its ethics approval; every questionnaire it reproduces may be reproduced (see the library topic in the forum); what it says about Steady is true of the current version.
3. **Zenodo:** the author makes a new upload (resource type "Publication / Preprint", licence CC BY 4.0, their ORCID), reserves the DOI, puts the DOI on the PDF's first page, uploads the PDF, asks for it to be in the `steadyapp` community and publishes. OpenWorks accepts it.
4. **Here:** a folder `content/papers/<short-name>/` with the PDF and an `index.md` (front matter as at the top of `layouts/papers/page.html`; the body is the paper's text in Markdown, which `pandoc paper.docx -t gfm` gets most of the way to). Date it the day of the Zenodo record. Open a pull request; check `/papers/` and the paper's page in `hugo server` on a phone and a computer.
5. **In the forum:** a reply on the paper's topic with its page and DOI.

A correction is a new version: a new version of the Zenodo record (same concept DOI), then the new PDF, `version` and `date` here, with what changed at the end of the paper.

## Running it locally

```bash
hugo server     # http://localhost:1313
```

Needs Hugo 0.146 or newer (extended not required). The workflow pins the version it builds with (`HUGO_VERSION`).

## Licence

Code: GNU AGPL v3 or later, like Steady. Fonts: Atkinson Hyperlegible Next and Barlow, SIL Open Font License (`static/fonts/`).
