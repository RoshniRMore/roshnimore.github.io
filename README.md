# Data scientist portfolio

A single-file portfolio (`index.html`) with light and dark themes, experience tabs, and a searchable, filterable project list. No build step and no dependencies.

## Customize

1. Update the availability line near the top of `index.html` (it is still a placeholder).
2. Edit the `jobs` and `projects` arrays at the bottom of the file. The experience tabs, project filters and filter counts update on their own.
3. Your photo is `assets/photo.jpg`. Your resume is deliberately NOT in this folder (see below).
4. Open `index.html` in a browser to preview.

## Deploy with GitHub Pages

```bash
cd portfolio-roshni
git init -b main
git add .
git commit -m "Add portfolio site"
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `(root)` → Save.**

A repo named `<your-username>.github.io` publishes at `https://<your-username>.github.io/`. Any other repo name publishes at `https://<your-username>.github.io/<repo-name>/`.

## Resume requests (approval flow)

Visitors click **Request resume**, fill in a short form, and it is emailed to you through Formspree (endpoint `xpwrkbdn`). In your Formspree dashboard, confirm that form delivers to `moreroshnir19@gmail.com`.

You approve by replying with the resume. Do not put the PDF in the repo: anything in a GitHub Pages repo is public. For the most control, share it from Google Drive with "Restricted" access and add only the approved person's email.
