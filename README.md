[README.md](https://github.com/user-attachments/files/32623666/README.md)
# Samridhi Papneja — Product Manager Portfolio

A single-page portfolio site showcasing 7 end-to-end PM case studies (Porter, Zomato, Twitter/X, Uber, Amazon, Myntra, and a B2B expense strategy), built as plain HTML/CSS/JS with no build step — so it deploys straight to GitHub Pages.

## What's inside

```
├── index.html                  ← the whole site (self-contained)
├── assets/
│   ├── resume/
│   │   └── Samridhi_Papneja_Resume.pdf
│   └── case-studies/
│       ├── 01-porter-first-trip-confidence.pdf
│       ├── 02-zomato-pm-strategy.pdf
│       ├── 03-twitter-x-aarrr-funnel.pdf
│       ├── 04-uber-find-my-ride.pdf
│       ├── 05-amazon-checkout-ux-audit.pdf
│       ├── 06-myntra-ux-analysis.pdf
│       └── 07-b2b-expense-strategy.pdf
```

## Before you publish: 2 things to fill in

1. **LinkedIn URL** — open `index.html`, search for `id="linkedinLink"`, and replace the `href="#"` with your actual LinkedIn URL. Update the link text too.
2. **Porter prototype / video links** — already wired up (`porter-first-trip-confidence-prototype-1.replit.app` and your Google Drive video). Double-check the Drive link's sharing setting is "Anyone with the link" so visitors can actually open it.

## Deploy to GitHub Pages (takes about 5 minutes)

1. **Create a repository.** Go to [github.com/new](https://github.com/new). Name it whatever you like — a common convention is `your-username.github.io` if you want it at the root of your GitHub domain, or any name (e.g. `pm-portfolio`) if you're fine with a `/repo-name/` path in the URL. Keep it Public.

2. **Upload these files.** Easiest way with no command line:
   - Open your new repo → "Add file" → "Upload files"
   - Drag in `index.html`, `README.md`, and the whole `assets` folder (drag the folder itself; GitHub preserves the structure)
   - Commit directly to the `main` branch

   Or with git, from this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
   git push -u origin main
   ```

3. **Turn on GitHub Pages.**
   - In your repo, go to **Settings → Pages**
   - Under "Build and deployment", set **Source** to "Deploy from a branch"
   - Set **Branch** to `main` and folder to `/ (root)`
   - Click **Save**

4. **Wait ~1–2 minutes**, then refresh that Pages settings page — it'll show your live URL, something like:
   - `https://your-username.github.io/your-repo-name/` (if you named the repo anything other than `your-username.github.io`)
   - `https://your-username.github.io/` (if you named it exactly `your-username.github.io`)

That's it — the site is live and free, and every time you push a change to `main`, it redeploys automatically.

## Making changes later

- **Swap or add a case study PDF**: drop the new file into `assets/case-studies/`, then update the matching `href` in `index.html`.
- **Add an 8th project**: copy one `.cs-card` block in `index.html` and edit the text, tag, and link.
- **Change colors/fonts**: everything is in the `<style>` block at the top of `index.html` under `:root` — the `--ink`, `--paper`, `--teal`, and `--gold` variables control the whole palette.

## Local preview

No build tools needed — just open `index.html` directly in a browser, or run a tiny local server from this folder:
```bash
python3 -m http.server 8000
```
then visit `http://localhost:8000`.
