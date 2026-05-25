# traitym-heart — static demo

This repository contains a small static heart-particles demo in the `heart/` folder.

Permanent hosting options
- GitHub Pages: after pushing to `main`, your site is published at:
  `https://<your-github-username>.github.io/<repo-name>/` — the repo root will now redirect to the demo at `/heart/external_5580_vi.html`.
- Netlify: if you connect this repository to Netlify, point the build publish directory to the repository root; Netlify will serve the same redirect and demo.

Quick verification
1. Push your changes to GitHub (commit + `git push`).
2. Visit `https://<your-github-username>.github.io/<repo-name>/` (it will redirect to `heart/external_5580_vi.html`).
3. If you prefer Netlify, connect the repo and deploy; the root URL will redirect to the demo as well.

If you'd like, I can:
- push these local changes to the remote for you and confirm the Pages URL, or
- set up a Netlify site and provide the Netlify URL.

Tell me which option you want me to perform next (push + confirm Pages, or set up Netlify deploy).

Netlify automatic deploy setup
- I added a `netlify.toml` (publish root) and a GitHub Action at `.github/workflows/netlify.yml`.
- To enable automatic deploys to Netlify, add these GitHub repository secrets:
  - `NETLIFY_AUTH_TOKEN` — create a Personal Access Token on Netlify (see Netlify docs).
  - `NETLIFY_SITE_ID` — the target Site ID from your Netlify site settings.
- After adding secrets, push to `main` and the Action will deploy the site to Netlify.

If you prefer, you can also connect the repository directly from the Netlify web UI (simpler): Netlify will create the site and set up builds automatically.
