# Coelia Ventures Website

The official website for **Coelia Ventures**, an independent product studio creating focused digital products that make complicated everyday information clearer and easier to use.

**Live website:** [https://coelia-bella.github.io/](https://coelia-bella.github.io/)

## Website structure

| Page | URL | Purpose |
| --- | --- | --- |
| Coelia Ventures | [`/`](https://coelia-bella.github.io/) | Company introduction, values, and featured work |
| Projects | [`/projects/`](https://coelia-bella.github.io/projects/) | Portfolio of products created by Coelia Ventures |
| PayScaleBD | [`/projects/payscalebd/`](https://coelia-bella.github.io/projects/payscalebd/) | Product overview, features, availability, and disclaimer |
| PayScaleBD Privacy | [`/projects/payscalebd/privacy/`](https://coelia-bella.github.io/projects/payscalebd/privacy/) | Full privacy policy presented as a webpage |
| PayScaleBD Support | [`/projects/payscalebd/support/`](https://coelia-bella.github.io/projects/payscalebd/support/) | Support contact, issue-reporting guidance, and privacy reminders |

The repository also includes a branded `404.html`, `robots.txt`, and `sitemap.xml`.

## Design system

The website follows the Coelia Ventures identity:

- **Coelia Navy:** `#081F36`
- **Coelia Champagne:** `#D6C4A8`
- **Coelia Ivory:** `#F6F0E6`
- **Coelia Graphite:** `#27313D`

The company pages use Coelia's editorial navy-and-champagne direction. PayScaleBD introduces its own green-and-gold product palette while remaining part of the same visual system.

Brand assets and the PayScaleBD app icon are stored in [`assets/`](assets/).

## Technology

The site is intentionally lightweight:

- Semantic HTML
- Responsive CSS
- Minimal vanilla JavaScript for navigation and reveal effects
- No package manager, framework, analytics, advertising, or external runtime dependencies
- Accessible keyboard navigation and reduced-motion support

All site paths are root-relative because this repository is published as the GitHub user site at `coelia-bella.github.io`.

## Repository layout

```text
.
├── index.html
├── 404.html
├── assets/
│   ├── styles.css
│   ├── site.js
│   ├── Coelia Ventures identity assets
│   └── PayScaleBD app icon
├── projects/
│   ├── index.html
│   └── payscalebd/
│       ├── index.html
│       ├── privacy/index.html
│       └── support/index.html
├── robots.txt
├── sitemap.xml
└── .github/workflows/pages.yml
```

## Preview locally

No installation or build step is required. From the repository root, start a local static server:

```sh
python3 -m http.server 4173
```

Then open [http://localhost:4173/](http://localhost:4173/).

Opening the HTML files directly with a `file://` URL is not recommended because the site uses root-relative asset and navigation paths.

## Deployment

The workflow in [`.github/workflows/pages.yml`](.github/workflows/pages.yml) publishes the repository to GitHub Pages whenever a commit is pushed to the `main` branch. Deployment can also be started manually from the repository's **Actions** page.

## Updating app availability

The PayScaleBD page links to the published app listings:

- **App Store:** [PayScaleBD for iOS](https://apps.apple.com/us/app/pay-scale-bd/id6819050160)
- **Google Play:** [PayScaleBD for Android](https://play.google.com/store/apps/details?id=com.coeliaventures.payscalebd)

Keep the store links in [`projects/payscalebd/index.html`](projects/payscalebd/index.html) pointed at the final public listings.

## Support

For website or PayScaleBD questions, contact [coelia.bella26@gmail.com](mailto:coelia.bella26@gmail.com).

Copyright © 2026 Coelia Ventures.
