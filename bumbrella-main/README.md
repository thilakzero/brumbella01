# Bumbrella-client2 — Site deployment

This repository contains a static website (index.html). To publish it via GitHub Pages the repository is prepared with a GitHub Actions workflow that deploys the repository root to the `gh-pages` branch whenever you push to `main`.

Follow these steps locally to push and trigger deployment:

1. Initialize git if not already initialized and set the remote to the repository URL:

```
git init
git add .
git commit -m "Initial site upload"
git branch -M main
git remote add origin https://github.com/apixymagic/Bumbrella-client2.git
```

2. Push to GitHub (you may be prompted for credentials or use a PAT):

```
git push -u origin main
```

3. GitHub Actions will run the `deploy` workflow and publish the site to the `gh-pages` branch. The Pages site URL will typically be:

```
https://apixymagic.github.io/Bumbrella-client2/
```

If you prefer to publish from the `main` branch directly via GitHub Pages settings, you can enable Pages from the repository settings and choose `main` / `/ (root)` as the publishing source.

If you want me to push the changes for you, provide a GitHub personal access token (PAT) or grant access; otherwise run the commands above locally.
