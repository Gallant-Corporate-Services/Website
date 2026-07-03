# Gallant Corporate Services Website

Static marketing site for Gallant Corporate Services.

## Project Structure

- `.nojekyll` keeps GitHub Pages from skipping underscore-prefixed files.
- `.gitignore` keeps generated local files out of the commit.
- `index.html` is the deployment entrypoint for GitHub Pages.
- `Gallant Home.dc.html` is the main landing page.
- `Gallant Group.dc.html` explains the parent company and structure.
- `Gallant Services.dc.html` lists the service lines and delivery process.
- `Gallant Divisions.dc.html` covers Gallant Branding International and Gallant Loop Africa.
- `Gallant Contact.dc.html` contains the contact form and office details.
- `Gallant Brand.dc.html` holds the brand guide and downloadable assets.
- `SiteNav.dc.html` and `SiteFooter.dc.html` are shared layout components.
- `support.js` provides the runtime used by the `.dc.html` pages.
- `assets/` contains logos, artwork, and other media used across the site.

## How The Site Is Wired

Each page loads `support.js`, then uses `dc-import` to pull in the shared navigation and footer. The pages are designed to work together as one site, with shared styling, shared navigation states, and consistent footer links.

## View Locally

Open `index.html` or `Gallant Home.dc.html` in a browser to start.

If your browser blocks any features when opening the file directly, serve the folder with any simple static server and open the home page from there.

## Before You Push To GitHub

- Make sure only the site files in this folder are staged.
- Check that `README.md` and `index.html` are included in the commit.
- If you publish with GitHub Pages, point the site to the repository root.

## Suggested Publish Steps

1. Review the changed files.
2. Commit the site files and this README.
3. Push to GitHub.
4. Publish from GitHub Pages or your preferred static host.

## Project Goal

The site presents Gallant as a single production partner with a clear brand, a shared service structure, and linked divisions under one roof.
