# American Politics 101 — website

Static site: `index.html`, `sessions.html`, `interview.html`, `reading.html`, `style.css`. No build step — plain HTML/CSS.

## Deploy to GitHub Pages (free)

1. Create the GitHub account (if you haven't already) at github.com.
2. Create a new repository — e.g. `american-politics-101`. Public, no README/gitignore needed (these files replace it).
3. Upload these five files to the repo:
   - On github.com, open the repo → **Add file → Upload files** → drag in `index.html`, `sessions.html`, `interview.html`, `reading.html`, `style.css` → **Commit changes**.
4. Turn on Pages: repo **Settings → Pages** → under "Build and deployment," set **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)** → **Save**.
5. GitHub builds the site (takes 1–2 minutes) and gives you a URL like `https://<your-username>.github.io/american-politics-101/`.

## One thing to check: Slides sharing

The Session 1 slide deck is embedded on `sessions.html` via an iframe pointing at Google Slides. For the embed to display (rather than an error), the presentation's sharing setting needs to be **"Anyone with the link" → Viewer**, not restricted:

Google Slides → **Share** → **General access** → change from "Restricted" to **"Anyone with the link"** → Viewer.

The download (.pptx) and "Open in Google Slides" buttons work regardless of this setting, as long as anyone who needs them has view access to the file.

## Adding Session 2 and 3 later

When those slide decks exist, edit `sessions.html`: duplicate the Session 1 block (heading, `<div class="embed-wrap">` iframe, and the two buttons), swap in the new presentation's file ID in all three URLs, and move that session out of the "Coming next" list.
