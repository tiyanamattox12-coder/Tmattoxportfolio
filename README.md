# Tiyana Mattox — Portfolio Site

Static site: `index.html` (Home), `projects.html`, `about.html`, `resume.html`, `resume.pdf`,
plus an `images/` folder holding all the photos. No build step — just plain HTML/CSS
files that link to each other and to files in `images/`.

## Get it live at a name-based URL (free, ~10 minutes)

**1. Create the repo**
Go to github.com/tiyanamattox12-coder → **New repository**.
Name it exactly: `tiyanamattox12-coder.github.io`
(This exact name — username + `.github.io` — is what makes GitHub host it at the root of your own URL instead of a `/repo-name/` sub-path.)
Keep it Public. Don't add a README from GitHub's UI (you already have one).

**2. Upload the files**
On the new repo's page, click **Add file → Upload files**, then drag in the whole downloaded folder — all the HTML files, `resume.pdf`, and the `images/` folder together (GitHub preserves the folder structure) — and commit. If drag-and-drop of a folder doesn't work in your browser, upload the HTML files and `resume.pdf` first, then click **Add file → Upload files** again and drag in just the `images` folder.

**3. Turn on Pages**
Repo → **Settings → Pages**. Under "Build and deployment," Source = **Deploy from a branch**, Branch = **main**, folder = **/(root)**. Save.

**4. Visit your site**
After a minute or two, it's live at:
**https://tiyanamattox12-coder.github.io**

That's your permanent link — share that one instead of the claude.ai link.

## Making updates later

- **Text edits**: open the file on GitHub, click the pencil icon, edit, commit — it redeploys automatically in ~1 minute.

- **Swap an existing photo without touching any code**: every photo on the site is loaded from the `images/` folder by filename (e.g. `images/headshot.jpg`, `images/cheer-action.jpg`). To replace one, just upload a new photo to the `images/` folder in your repo **with that exact same filename** — GitHub will ask "replace existing file?" and the site updates automatically, no HTML editing needed.

- **Add a brand-new photo (a new filename)**: upload it to `images/` with any name, then open the relevant HTML file, find the `<img src="images/...">` line for that section, and change the filename inside the quotes to match.

- **Add a project to the home page carousel**: in `index.html`, search for the comment `FEATURED CAROUSEL`, copy one whole `<article class="pcard">...</article>` block, paste it inside `<div class="carousel-track">`, and edit its text and photo path.

- **Add a project to the Projects page**: in `projects.html`, search for the comment `TO ADD A NEW PROJECT`, copy one whole `<div class="card">...</div>` block, and edit it. That comment also explains the three photo layouts a card can use (two photos side by side, one photo, or a placeholder).

- **Add an activity to the About page**: in `about.html`, copy one whole `<div class="entry">...</div>` block and edit it.

- **Update your resume**: upload a new `resume.pdf` over the old one (same filename), and the download button keeps working.

- Anytime you'd rather not touch the code yourself, send me the change (and any new photos) and I'll edit the files for you — just re-download and re-upload them to GitHub.

## Optional: a custom domain later
If you ever buy a domain (e.g. `tiyanamattox.com`), GitHub Pages supports pointing it at this same repo — just ask and I'll walk you through the DNS + repo settings.
