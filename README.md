# Gabriel Ping-ay — Portfolio

A responsive, single-page portfolio with seven page-like views. It uses plain HTML, CSS, and JavaScript, so it has no build step or dependencies.

## Files

All website files are in this folder’s root, so you can upload them directly to the root of your GitHub repository:

- `index.html` — page content
- `style.css` — visual design
- `script.js` — navigation and interactions
- `profile.jpg` — supplied homepage portrait
- `voxel-forest.svg` — Minecraft-inspired pixel forest
- `grass-block.svg` — pixel grass block artwork
- `enchanting-table.svg` — purple enchanted table artwork
- `profile-placeholder.svg` — portrait fallback
- `favicon.svg` — browser tab icon

## Run locally

Open `index.html` in a modern browser. For a local web server, run `python -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Add all the files in this folder to the root of your GitHub repository.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**, choose your publishing branch (usually `main`) and the `/ (root)` folder, then save.
4. Wait for GitHub Pages to publish and use the URL shown in the Pages settings.

## Optional custom `www` domain

You need to own a domain name and have access to its DNS settings. In GitHub Pages settings, enter the exact hostname you want, such as `www.example.com`. At your DNS provider, create a `CNAME` record whose host/name is `www` and whose target/value is `YOUR-USERNAME.github.io` (replace this with your GitHub account’s Pages hostname; do not include a repository path). Allow DNS time to update, then return to Pages settings and enable HTTPS when it becomes available. A `www` hostname points to the GitHub Pages hostname using the CNAME record; it does not by itself purchase a domain or provide the bare `example.com` address. To use the bare domain too, configure the DNS records GitHub documents for apex domains and optionally redirect between the two hostnames.

## Site controls

- Use the top navigation or the Previous/Next buttons to move between all seven views.
- The arrow keys also change views when focus is not on a control.
- Select a skill card to reveal an additional note.
- On desktop the portfolio fits in the viewport; on smaller screens the content can scroll naturally.

The content avoids claiming awards, certificates, named projects, or developer accounts that have not been provided.
