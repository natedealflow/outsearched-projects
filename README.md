# OutSearched Client Results

Static one-page site: client case studies for OutSearched.

- `index.html` is the whole site (logos are embedded, no build step).
- Hosted on Vercel. Every push to `main` redeploys automatically.

## Landing page videos

Files live in `/videos`. Filenames carry a version (`main-v1.mp4`), so a new cut gets a new name (`main-v2.mp4`) instead of overwriting; `vercel.json` tells browsers to cache them for a year.

- `main-v1.mp4`: main landing page video (1080p, captions burned in)
- `main-v1-poster.jpg`: still shown before play
- `main-v1.vtt`: transcript captions (optional, the video already shows captions)

Embed (replace DOMAIN with the Vercel domain):

```html
<video src="https://DOMAIN/videos/main-v1.mp4" poster="https://DOMAIN/videos/main-v1-poster.jpg"
  controls playsinline preload="metadata" style="width:100%;height:auto;border-radius:8px;display:block"></video>
```
