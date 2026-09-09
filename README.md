# Andrew Hanna Photography — portfolio site

Static site: `index.html` + `img/` (full size) + `thumb/` (grid) + logo files. No build step, no server needed.

## Publish on GitHub Pages (free) — about 5 minutes

1. Go to https://github.com and sign in (create a free account if needed).
2. Click **New repository**. Name it `andrewhanna-photography` (or `<your-username>.github.io` for the shortest URL). Public. Click **Create repository**.
3. On the empty repo page click **uploading an existing file**. Drag ALL the contents of this folder in (index.html, README.md, .nojekyll, the img and thumb folders, the png/jpg files). Click **Commit changes**.
   - If the browser won't let you drag folders, upload `index.html` and the loose files first, then open the `img` and `thumb` folders and drag their files in one folder at a time (GitHub keeps the folder name if you drag the folder itself in Chrome).
4. Repo **Settings → Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch **main**, folder **/ (root)**. Save.
5. Wait ~1 minute. Your site is live at `https://<your-username>.github.io/andrewhanna-photography/` (or `https://<your-username>.github.io/` if you used that repo name). Put that link in your Instagram bio.

Custom domain later: buy e.g. `andrewhanna.photo`, add a CNAME record pointing to `<your-username>.github.io`, then enter the domain under Settings → Pages → Custom domain.

## Updating photos
Drop a JPG into `img/` and a smaller copy (≤720px) into `thumb/`, then add one line to the `ITEMS` array near the bottom of `index.html`:
`{"src":"img/name.jpg","thumb":"thumb/name.jpg","cat":"auto","w":1080,"h":720}`
Categories: auto, events, interiors, portraits, food, city.
