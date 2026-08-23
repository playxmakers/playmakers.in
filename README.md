# Playmakers Portfolio

A single-page portfolio site (Architecture / Urbanism / Landscape / Geomatics) — all images are embedded as base64, so it's just one self-contained `index.html` file.

## Publish with GitHub Pages

1. **Create a new repository** on GitHub (e.g. `playmakers-site`). Don't initialize it with a README (you already have one here).

2. **Upload the file** — easiest way, no git needed:
   - Go to your new repo → **Add file → Upload files**
   - Drag in `index.html` and `README.md` from this folder
   - Commit directly to the `main` branch

   *(Or via git, if you prefer the command line:)*
   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repo → **Settings → Pages**
   - Under "Build and deployment" → **Source**, select **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)` → **Save**

4. **Wait ~1 minute**, then your site will be live at:
   ```
   https://<your-username>.github.io/<your-repo>/
   ```

## Notes

- The file is ~18MB (all project images are embedded inline as base64 so there are no separate image files to manage). GitHub's per-file limit is 100MB, so this is well within range.
- If you'd rather use a custom domain, add a `CNAME` file to the repo root with your domain name, and point your DNS to GitHub Pages per [GitHub's docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
