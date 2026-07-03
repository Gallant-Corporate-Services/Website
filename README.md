# Gallant Corporate Services Website

Static website for Gallant Corporate Services.

The site opens from `index.html`, which sends visitors to the home page.

## Project structure

- `Gallant Home.dc.html` is the landing page.
- `Gallant Group.dc.html` explains the company structure.
- `Gallant Services.dc.html` lists the service lines and process.
- `Gallant Divisions.dc.html` covers Gallant Branding International and Gallant Loop Africa.
- `Gallant Contact.dc.html` contains the enquiry form and office details.
- `Gallant Brand.dc.html` holds the brand guide and asset references.
- `SiteNav.dc.html` and `SiteFooter.dc.html` are shared layout components.
- `support.js` provides the runtime used by the `.dc.html` pages.
- `assets/` contains logos, images, and supporting files.

## How it works

Each page loads `support.js`, then uses `dc-import` to pull in the shared navigation and footer. The pages share the same visual system, navigation state, and footer links so the site feels like one connected project.

## Local use

Open `Gallant Home.dc.html` in a browser to view the site.

If you want to serve it locally, use any simple static server from this folder and open the home page from that server.

## GitHub Pages note

The repository includes a `.nojekyll` file so GitHub Pages serves files that start with an underscore, including the generated asset sheet under `assets/logos/`.

## Before pushing

1. Review the changed files.
2. Stage only the site files and root configuration files.
3. Commit the changes.
4. Push to `origin` on the current branch.