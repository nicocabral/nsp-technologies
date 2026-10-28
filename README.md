# NSD Technologies — company website

A single-page marketing site for **NSD Technologies**, a software studio
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

> GitHub Pages is free **only on public repositories**. If this repo is
> private, open **Settings → General → Danger Zone → Change repository
> visibility → Make public** first. (The site contains no secrets.)

1. Commit and push these files to the repository (e.g. the `main` branch).
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Branch: **main**, folder: **/ (root)**. Save.
5. Wait ~1 minute. Your site goes live at
   `https://nicocabral.github.io/nsp-technologies/`.

### Custom domain (optional)

To serve it from your own domain (e.g. `nsdtech.ph`):

1. Add a file named `CNAME` containing just the domain, e.g. `nsdtech.ph`.
2. At your domain registrar, point the domain to GitHub Pages
   (a `CNAME` record to `nicocabral.github.io`, or `A` records to
   GitHub's Pages IPs).
3. In **Settings → Pages**, enter the custom domain and enable
   **Enforce HTTPS**.

## Renaming the repository (optional)

The repo is currently named `nsp-technologies`. To match the new brand, you
can rename it to `nsd-technologies` in **Settings → General → Repository
name**. GitHub keeps redirects from the old name, and the Pages URL becomes
`https://nicocabral.github.io/nsd-technologies/`. The folder on your computer
can be renamed too; update the git remote if you do.

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
