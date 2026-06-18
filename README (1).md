# VeriSight AI Prototype

This is a static browser prototype for a deepfake and AI-content authenticity product.

## Files

- `index.html`: the full working prototype

## What the prototype includes

- upload and preview for image, audio, and video
- browser-based authenticity scoring flow
- explainability output with signal bars and reasons
- live camera simulation mode
- JSON export for the analysis result

## Run locally

You can open `index.html` directly in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Publish online

Because this is a static site, you can publish it on any static host.

### Netlify

1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag the project folder or the `index.html` file into the upload area
3. Netlify will generate a public URL

### Vercel

1. Create a new project in [Vercel](https://vercel.com/)
2. Import the folder or upload it through a Git repository
3. Deploy it as a static site

### GitHub Pages

1. Create a GitHub repository
2. Upload `index.html` and `README.md`
3. Enable GitHub Pages for the root branch
4. GitHub will give you a public URL

## Important note

This version is a prototype for demos and presentations. It does not use production ML models yet. The scoring logic is generated in the browser to simulate a realistic trust-and-safety workflow.

## Suggested next step

If you want a production-like version, replace the browser scoring logic with:

- an image detection API
- a voice analysis API
- a video temporal-consistency API
- a backend that stores reports and user submissions
