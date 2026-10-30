# sigma-website

The website for **Sigma Explains** (sigmaexplains.com), a YouTube channel that teaches math and statistics Where → Why → What, hosted by Sigma and his family of co-hosts.

It's a static site: plain HTML and CSS with no build step and no dependencies.

```
index.html          the page
styles.css          all styles (responsive: phone, tablet, desktop)
assets/favicon.svg  Σ icon
assets/cast/*.webp  character art (Sigma, Delta, Theta, Grandma Mu, Epsilon, Pi, Lambda, full lineup)
```

## Run it locally
Open `index.html` in a browser, or run:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Change the YouTube link
Every YouTube button reads its link from one line near the bottom of `index.html`:

```js
const YOUTUBE_URL = "https://www.youtube.com/@SigmaExplainsMath";
```

## Publish on GitHub Pages
1. In the repo, go to **Settings → Pages**.
2. Set **Source** to *Deploy from a branch*, then choose `main` and `/ (root)`.
3. To use your own domain, enter `sigmaexplains.com` under **Custom domain**, then point the domain's DNS to GitHub Pages.
