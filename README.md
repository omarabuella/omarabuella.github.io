# Prof. Omar Abu-Ella — Academic Website

A bilingual Arabic/English academic website extracted from the supplied July 2026 CV. It is a dependency-free static site, optimized for fast loading and suitable for GitHub Pages, Netlify, Cloudflare Pages, or a university server.

## Preview locally

Run this command from the website folder:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Before public launch

1. Replace `assets/profile-placeholder.svg` with the official portrait. Keep the same filename or update the image path in `index.html`.
2. The canonical URL, language alternates, robots file, and sitemap use the public URL `https://omarabuella.github.io/`.
3. Update the citation figure only from the verified Google Scholar profile. The current interface deliberately links to the live Scholar profile instead of freezing an unverified count.
4. Verify the Scopus and Web of Science author IDs. The current buttons intentionally open author-search pages because stable author identifiers were not present in the supplied CV.
5. Add student names, degree status, thesis repository links, project funding, partners, and teaching-material downloads when those data are supplied. The CV lists topics but does not provide these details.
6. For a server-side contact form, connect a privacy-respecting service or university endpoint. The included form creates a local `mailto:` message and stores no personal data.

## Content updates

- Publications, research areas, teaching, profiles, and bilingual text: `app.js`
- Layout and metadata: `index.html`
- Colors, typography, responsive behavior, and print style: `styles.css`
- Downloadable CV: `assets/Omar_Abu-Ella_CV_2026.pdf`

## GitHub Pages deployment

1. Create a public repository and upload the contents of this folder to its root.
2. In **Settings → Pages**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
3. Keep the canonical and sitemap entries synchronized if the site later moves to a custom domain.
4. If using a custom domain, add a `CNAME` file containing only the domain name and configure DNS with the domain provider.

## Included quality features

- Arabic RTL and English LTR with a persistent language toggle
- Responsive navigation and layouts for mobile, tablet, and desktop
- Dark mode, reduced-motion support, keyboard skip link, accessible labels
- Searchable/filterable complete publication list
- Person JSON-LD, Open Graph metadata, sitemap, robots file, and canonical URL
- No web fonts, trackers, external scripts, or large framework bundles
- Print-friendly CSS and downloadable CV

## Source accuracy

Biographical, teaching, supervision, service, and publication information comes from `Omar_Abu-Ella_CV_2026.tex` and the accompanying IEEE biography. DOI/profile links were checked where publicly identifiable. No citation total, student identity, funding amount, or partnership was invented.
