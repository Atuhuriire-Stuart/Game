# Game
Enjoy the game

## Deploying to GitHub Pages

This repository is a static site (contains `index.html`). There are two simple ways to publish it to GitHub Pages:

- **Automatic (recommended)**: I added a GitHub Actions workflow that publishes the repository root to GitHub Pages on every push to `main`.

	- Workflow file: `.github/workflows/gh-pages.yml`
	- After you push the workflow to the `main` branch, GitHub Actions will run and publish the site.

- **Manual (via repository settings)**: In the repository on GitHub, go to **Settings → Pages**, choose the `main` branch and `/ (root)` folder (or the `gh-pages` branch if you prefer), then save.

### How to enable/publish (commands)

1. Commit and push the workflow and any changes:

```bash
git add .github/workflows/gh-pages.yml README.md
git commit -m "Add GitHub Pages deploy workflow and instructions"
git push origin main
```

2. Wait for the Actions run to finish: open the **Actions** tab in the GitHub repo and confirm the workflow completed successfully.

3. Your site will be available at:

```
https://Atuhuriire-Stuart.github.io/Game/
```

If you use a custom domain, configure it in **Settings → Pages** and add a `CNAME` file to the repo root with your domain.
