# 🎬 Say It Like the Movies

A simple website to practice English speaking with famous movie quotes.

Pick a quote, listen to it, say it into your microphone, get a score, then watch the original scene.

## Features
- 40 famous movie quotes (single lines and multi-sentence ones), tagged Easy / Medium / Hard
- ← Prev / Next → buttons to practice quote after quote
- + Add your own sentences (one per line), saved in the browser
- Search by quote or movie name
- 🔊 Listen (normal and slow) using the browser's text-to-speech
- 🎤 Speaking check with a % score and word-by-word feedback
- ⌨️ Type-what-you-said fallback if the microphone is unavailable
- ▶ Link to find the movie clip on YouTube (or embed it directly)
- Progress saved in the browser (localStorage)
- Light and dark mode

## Run locally
No build step. Open `index.html` in Chrome or Edge.

## Add quotes
Edit the `BASE` list in `index.html`:

```js
["Quote text.", "Movie title", "Year", "Character", "YOUTUBE_VIDEO_ID"],
```

Leave the last field empty (`""`) to show a "Find the movie clip" link. Add a YouTube video ID to embed the clip inside the page.

## Deploy with GitHub Pages
1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. Your site will be live at `https://<username>.github.io/movie-quotes-practice/`.

## Notes
- Speech recognition works in Chrome and Edge, over HTTPS (GitHub Pages is HTTPS).
- Movie quotes belong to their respective owners. This project is for educational use and links to YouTube instead of hosting any video.

## Tech
HTML, CSS, vanilla JavaScript, Web Speech API.
