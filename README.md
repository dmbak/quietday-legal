# quietday-legal

Static website for the [QuietDay](https://apps.apple.com/app/quietday) iOS app, served via GitHub Pages. Contains the landing page, Privacy Policy, Terms of Use, and Support page.

## Repository structure

```
/
├── index.html      Landing page
├── privacy.html    Privacy Policy
├── terms.html      Terms of Use
├── support.html    Support & FAQ
├── assets/
│   └── style.css   Shared styles (no framework, no JavaScript)
└── README.md
```

## GitHub Pages setup

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select **Deploy from a branch**.
4. Choose the `main` branch and `/ (root)` folder.
5. Click **Save**.

GitHub Pages will serve the site at `https://<your-username>.github.io/<repo-name>/`. To use a custom domain (e.g. `legal.quietday.app`), add a `CNAME` file containing your domain and configure your DNS provider.

## Updating policy pages

All content is plain HTML. To update a policy:

1. Open `privacy.html` or `terms.html` in any text editor.
2. Edit the relevant section inside the `<div class="prose">` block.
3. Update the **Effective date** in the `<p class="page-meta">` line near the top.
4. Commit and push — GitHub Pages redeploys automatically within a minute.

No build step, no dependencies, no framework required.
