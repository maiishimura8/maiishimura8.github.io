# Mai Ishimura — 石村眞愛

Personal portfolio website. Plain HTML, CSS and JavaScript, so there is no build step: GitHub Pages serves these files as they are.

## Files

| File | Page |
| --- | --- |
| `index.html` | Main page: shoji entrance, intro, Projects, About Me, Contact |
| `research.html` | Research |
| `architecture.html` | Architecture sketchbook |
| `activities.html` | Activities |
| `graphic-design.html` | Graphic design |
| `assets/` | Photos, textures, posters and résumé PDFs |

## Publish with GitHub Pages

1. On github.com, click **New repository**.
   - Name it `YOUR-USERNAME.github.io` for the site to live at `https://YOUR-USERNAME.github.io`.
   - Any other name, e.g. `portfolio`, puts it at `https://YOUR-USERNAME.github.io/portfolio`.
   - Make it **Public**, then **Create repository**.
2. On the new repo page, click **uploading an existing file**. Drag in everything inside this folder, the `assets` folder included, then **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**, then **Save**.
4. Wait a minute or two and refresh the Pages settings. The live link appears at the top.

### Using the command line instead

```bash
cd mai-ishimura-site
git init
git add .
git commit -m "Publish portfolio site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

Then do step 3 above.

## Custom domain (maiishimura.com)

1. In **Settings → Pages → Custom domain**, enter `maiishimura.com` and save. GitHub adds a `CNAME` file to the repo.
2. At your domain registrar, add these DNS records:
   - Four **A** records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One **CNAME** record for `www` pointing to `YOUR-USERNAME.github.io`
3. Once the domain shows as verified, often within an hour though DNS can take up to a day, tick **Enforce HTTPS**.

## Editing later

- **Text:** open the page's `.html` file on GitHub, click the pencil icon, change the words and commit. The site updates in about a minute.
- **A photo:** upload the new image to `assets/` with the same file name as the old one, or change the `src="assets/…"` in the HTML.
- **The entrance:** it plays once per browser visit. Linking straight to a section, such as `index.html#projects`, skips it. The **Replay entrance** button in the menu plays it again.
