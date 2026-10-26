# Personal Academic Researcher Homepage

A minimal, responsive researcher website made with plain HTML, CSS, and JavaScript. Ready for GitHub Pages.

## 1. Personalize before publishing

Open `index.html` and search/replace:

- `Your Name` and initials `YN`
- `your.email@example.com`
- Institution, lab, current position, and location
- Google Scholar, GitHub, and LinkedIn URLs
- Publication author list, venue, official status, DOI, paper/code/dataset URLs
- Project descriptions and repository links
- News entries and research interests

**Accuracy note:** The included biography and project summaries are starter text. Keep only claims that accurately represent your role and current work. Confirm the official publication metadata and author order before making the page public.

## 2. Add a portrait

Put a portrait image at `assets/profile.jpg`. To use it, replace the `.portrait-placeholder` element in `index.html` with:

```html
<img class="portrait-image" src="assets/profile.jpg" alt="Portrait of Your Name">
```

Then add this rule to `styles.css`:

```css
.portrait-image {
  display: block;
  width: 100%;
  aspect-ratio: 4 / 4.6;
  object-fit: cover;
  object-position: center;
}
```

Use an image you have permission to publish.

## 3. Add your CV

Place your public PDF at `assets/cv.pdf`. The CV links already point there. If you do not want to publish a CV yet, remove the two CV links in `index.html`.

## 4. Preview locally

Open `index.html` in a browser. For a local server, from this folder run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## 5. Publish with GitHub Pages

1. Create a GitHub repository named exactly `YOUR-USERNAME.github.io`.
2. Upload the contents of this folder (the files should be at the repository root).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main`, folder `/(root)`, then save.
6. Wait for the Pages deployment to finish. Your site will be at `https://YOUR-USERNAME.github.io`.

See the official guide: https://docs.github.com/en/pages/quickstart

## 6. Optional custom domain

You can later connect a domain from **Settings → Pages → Custom domain** and follow GitHub's DNS instructions.

## Files

- `index.html` — homepage content and structure
- `styles.css` — layout, typography, colors, mobile behavior
- `script.js` — responsive navigation and footer year
- `assets/` — place your portrait and CV here
