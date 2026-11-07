# Portfolio template

A one-page portfolio with project write-up pages. Plain HTML and CSS, one optional script, no build step, no dependencies. Light and dark themes follow the visitor's system setting.

**Live demo:** https://alan-haddad.github.io/portfolio-template/

## What's included

| Path | What it is |
| --- | --- |
| `index.html` | Home page: hero, about, work, experience, credentials, contact |
| `project.html` | Write-up page for one project. Copy it once per project |
| `404.html` | Not-found page (GitHub Pages serves it automatically) |
| `favicon.svg` | Placeholder browser-tab icon |
| `assets/css/site.css` | All styles. Design tokens (colours, fonts, widths) are at the top |
| `assets/js/reveal.js` | Scroll-in animation. Optional: the page works without it |
| `assets/fonts/` | Self-hosted Mona Sans and Geist Mono (SIL Open Font License, see `OFL.txt`) |
| `LICENSE` | MIT License for the template code |
| `.github/workflows/static.yml` | Deploys the site to GitHub Pages on every push to `main` |

## Make it yours

1. **Search for "Your Name" and "EDIT"** across the HTML files and replace them. Every editable spot has a comment explaining it.
2. **Hero.** Name, one or two lines of role, and the code window. Replace the window's lines with something from your field, or delete the `.stage-shot` block for a text-only hero.
3. **About.** The two-tone statement (the `<span>` part renders lighter), three short paragraphs, four highlight tiles.
4. **Work.** One full-width featured project and two smaller ones. Each links to a write-up page. Copy `project.html` to something like `my-project.html` for each, and update the links.
5. **Experience.** Newest first. There are three entry styles: a standard role, a company with several roles, and a one-line entry for older history.
6. **Credentials.** Four cards plus an education line. Rename the section if "Certifications" or "Awards" fits better (update the nav link too).
7. **Contact.** Your links. For email, use `href="mailto:you@example.com"`, or leave email off and point people to LinkedIn.
8. **Share image.** Add a 1200×630 `images/og.png` and uncomment the `og:image` lines so links look good on LinkedIn and in messages.
9. **Favicon.** Replace the placeholder mark in `favicon.svg`.
10. **URLs.** Replace `https://example.com/` in the `canonical` and `og:url` tags with your site's address.

## Change the look

Everything visual comes from the tokens at the top of `assets/css/site.css`:

- `--accent` is the link and button colour (with a lighter version in the dark-mode block).
- `--signal` and `--amber` are the highlight colours used in diagrams and the code window.
- `--stage` is the black background behind the hero, contact section and write-up headers.
- `--font` and `--mono` set the typefaces. Swap the files in `assets/fonts/` and the `@font-face` rules to change them.

## Publish on GitHub Pages

1. Create a repository named `your-username.github.io` and push these files to its `main` branch.
2. In the repository, go to **Settings → Pages** and set **Source** to **GitHub Actions**.
3. The included workflow deploys every push to `main`. The site appears at `https://your-username.github.io/` within a minute or two.
4. Optional: add a custom domain under **Settings → Pages → Custom domain**, then update the `canonical` and `og:url` tags.

If you use a different repository name, the site lives under `/repo-name/`. Everything works there except `404.html`, whose paths start with `/`; prefix them with `/repo-name`.

To preview locally, open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit `http://localhost:8000`.

## Accessibility and performance

Already handled: a skip link, semantic landmarks, labelled diagrams, visible focus styles, reduced-motion support, content that stays visible without JavaScript, self-hosted fonts with `font-display: swap`, and a layout that works down to 320px wide. Keep `alt` text on any images you add and `<title>`/`<desc>` on any diagrams.

## License

The template code (HTML, CSS, JS) is released under the MIT License, see `LICENSE`. You can use and change it freely for your own site; keep the `LICENSE` file in your copy. The fonts are under the SIL Open Font License, see `assets/fonts/OFL.txt`.
