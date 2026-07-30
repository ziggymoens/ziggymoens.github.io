# ziggymoens.github.io

Personal site of Ziggy Moens, Odoo solution architect. Live at [ziggymoens.github.io](https://ziggymoens.github.io/).

## How it works

One page, one file. `index.html` contains the markup, the CSS and the ~30 lines of JavaScript that
handle the sticky header, scroll spy and reveal-on-scroll. There is no build step, no framework and
no dependency beyond a Google Fonts stylesheet. Open the file in a browser and what you see is what
gets deployed.

## Structure

```
├── index.html            → the entire site
├── assets/img/           → portrait, OG image and logos
├── sitemap.xml           → SEO sitemap
└── README.md
```

## Editing

- **Content** lives in the `<main>` element, split into the sections `about`, `work`, `education`,
  `expertise` and `contact`.
- **Theming** runs on CSS custom properties in `:root`, with a dark variant under
  `@media (prefers-color-scheme: dark)`. Changing `--accent` restyles the whole page.
- **Diplomas and certificates** are not stored here. They live in
  [ziggymoens/ziggymoens](https://github.com/ziggymoens/ziggymoens) and are linked from the
  education cards.

## Deployment

GitHub Pages serves `main` directly. Push to `main` and the change is live within a minute.
