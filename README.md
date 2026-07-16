# Gallant Corporate Services Website

Static website for Gallant Corporate Services.

The site is served with clean URLs (no `.html` anywhere in a link): each page lives in its own folder as `index.html`, so it's reachable at a plain path like `/group/`.

## Project structure

- `index.html` (root) is the home page.
- `group/index.html` explains the company structure.
- `services/index.html` lists the service lines and process.
- `divisions/index.html` covers Gallant Branding International and Gallant Loop Africa.
- `contact/index.html` contains the enquiry form and office details.
- `brand/index.html` holds the brand guide and asset references.
- `brand/print/index.html` is an unlinked print-formatted copy of the brand guide.
- `SiteNav.dc.html` and `SiteFooter.dc.html` are shared layout components, fetched at runtime from the site root regardless of which folder the current page is in.
- `support.js` provides the runtime used by every page; `image-slot.js` supports the photo-slot placeholders on the Services/Divisions pages.
- `assets/` contains logos, images, and supporting files. All pages reference assets and scripts with root-absolute paths (e.g. `/assets/...`, `/support.js`) so they resolve correctly no matter how deep the page's folder is.

## How it works

Each page loads `support.js`, then uses `dc-import` to pull in the shared navigation and footer from `/SiteNav.dc.html` and `/SiteFooter.dc.html`. The pages share the same visual system, navigation state, and footer links so the site feels like one connected project.

## Local use

Serve this folder with any static server (e.g. `python3 -m http.server`) and open `/` — opening `index.html` directly via `file://` will break the root-absolute asset paths.

## GitHub Pages note

The repository includes a `.nojekyll` file so GitHub Pages serves files that start with an underscore, including the generated asset sheet under `assets/logos/`.

## Before pushing

1. Review the changed files.
2. Stage only the site files and root configuration files.
3. Commit the changes.
4. Push to `origin` on the current branch.
