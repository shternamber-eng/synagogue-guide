# Lubavitch Historical Archive Project

Static, responsive informational site with structured data files for history, restoration, gallery, news, archive, and contact.

## Run locally
Open `index.html` with a local web server (recommended):
- `python3 -m http.server 4173`
- Visit `http://localhost:4173`

## Add a new gallery image
1. Add image file to `public/images/gallery/`.
2. Add a new item in `data/gallery.json` with fields: `id,title,image,category,date,location,caption,description,credit,alt,tags`.

## Add a news update
1. Add a new object in `data/news.json`.
2. Include `slug` and `coverImage`.
3. Open via `news-item.html?slug=your-slug`.

## Edit restoration timeline
Update `data/restoration.json` (`year,date,title,description,category,status,images,source,notes,relatedGalleryItems`).

## Replace placeholder images
Replace files in:
- `public/images/hero/`
- `public/images/gallery/`
- `public/images/sites/`
- `public/images/news/`
- `public/images/archive/`

## Deploy
- **Cloudflare Pages / Netlify**: publish root directory as static site.
- **Vercel**: import as static project, output directory `.`.

## Notes
- Historical facts must be verified before final publication.
- Do not publish personal data without permission.
