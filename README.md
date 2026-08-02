# tschmah.github.io — setup notes

## Publishing on GitHub Pages

1. On GitHub, create a new repository named exactly `<your-username>.github.io`
   (e.g. if your GitHub username is `tschmah`, the repo must be named
   `tschmah.github.io`). This exact naming is what makes GitHub serve it as a
   user site at `https://<your-username>.github.io/` with no extra config.
2. Upload these files (`index.html`, `research.html`, `teaching.html`,
   `publications.html`, `style.css`, and the `images/` folder) to the root of
   that repository — either via the GitHub web UI ("Add file" → "Upload
   files") or via `git`.
3. In the repo, go to Settings → Pages, and confirm the source is set to
   deploy from the `main` branch, root folder. (Usually this is automatic
   once index.html is in the root.)
4. Wait a minute or two, then visit `https://<your-username>.github.io/`.

## Things to fill in before/after publishing

- `images/photo.jpg` — add a current headshot (the folder is currently
  empty).
- `CV.pdf` — add your CV if you want the "CV" link on the home page to work,
  or delete that line.
- Office room number on the home page.
- Current-term courses on the teaching page.
- `Schmah_Undergrad_Projects.pdf` on the research page, or update/remove that
  link.
- The "Last modified" line at the bottom of each page — I've left an HTML
  comment (`<!-- update date -->`) as a marker; just edit the visible text
  next to it.

## Custom domain (optional, later)

If you ever want something like `www.tanyaschmah.com` instead of the
`github.io` address, you'd buy the domain from a registrar and add a `CNAME`
file to the repo pointing to it — GitHub Pages supports this natively. Not
needed for now.
