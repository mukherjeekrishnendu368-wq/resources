# ISI & CMI Entrance Resources

A static website hosting a curated collection of preparation materials for the
**ISI (B.Stat / B.Math)** and **CMI** entrance examinations — past papers,
handouts, quick-revision summaries, problem collections, and mock tests.

## Live site

Once deployed via GitHub Pages, the site is available at:
`https://<your-username>.github.io/<repo-name>/`

## Structure

```
.
├── index.html        # the site (single page, all sections)
├── .nojekyll         # tells GitHub Pages to serve files as-is
├── pdfs/             # all resource PDFs
└── README.md
```

## Deploying to GitHub Pages

1. Create a new repository on GitHub (public).
2. Upload every file and folder here (`index.html`, `.nojekyll`, `pdfs/`, `README.md`)
   to the repository — either through the web uploader or with git:

   ```bash
   git init
   git add .
   git commit -m "Add ISI-CMI entrance resources site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/ (root)**, then **Save**.
6. Wait ~1 minute; your site will be live at the URL shown on that page.

## Updating

To add or remove a resource, drop the PDF into `pdfs/` and add a matching
`<a class="card" ...>` entry inside the relevant `<section>` in `index.html`.
