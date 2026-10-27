# NSP Technologies — company website

A single-page marketing site for **NSP Technologies**, a software studio
building operations software for Philippine businesses. It showcases our two
products:

- **Gatherly** — all-in-one platform for events & catering businesses · [gathery.space](https://gathery.space)
- **EduFlow** — complete school management system · [gatp.app](https://gatp.app)

The site is a single static `index.html` (no build step, no dependencies).
Fonts load from Google Fonts; everything else is self-contained.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire website |
| `favicon.svg` | Browser-tab icon (the `_>` mark) |
| `.nojekyll` | Tells GitHub Pages to serve files as-is (no Jekyll processing) |
| `og-image.png` | *(optional)* social share image for Facebook/Twitter link previews |

## Publishing with GitHub Pages

1. Commit and push these files to the repository (e.g. the `main` branch).
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Branch: **main**, folder: **/ (root)**. Save.
5. Wait ~1 minute. Your site goes live at
   `https://<your-username>.github.io/nsp-technologies/`.

### Custom domain (optional)

To serve it from your own domain (e.g. `nsptech.ph`):

1. Add a file named `CNAME` containing just the domain, e.g. `nsptech.ph`.
2. At your domain registrar, point the domain to GitHub Pages
   (a `CNAME` record to `<your-username>.github.io`, or `A` records to
   GitHub's Pages IPs).
3. In **Settings → Pages**, enter the custom domain and enable
   **Enforce HTTPS**.

## Facebook link previews

For a rich preview card when the link is shared on Facebook, add an
`og-image.png` (1200×630px) to this folder — the `<meta property="og:image">`
tag already references it. Without it, Facebook shows a plain text link.

## Editing

Open `index.html` in any editor. Content is organized top to bottom:
nav → hero → studio → Gatherly → EduFlow → why → contact → footer.
Colors and type are defined as CSS variables in the `:root` block at the top
of the `<style>`.

## Contact

ncabral010694@gmail.com
