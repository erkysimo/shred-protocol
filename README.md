# Shred Protocol

A meal prep PWA for a 3-day Bangkok cutting plan (~1,700 kcal, 153g protein). Includes meal plans, grocery list with real Thai prices, AI receipt scanner (Claude), and monthly budget tracker.

---

### 🚀 One-time setup (do this once)

1. Fork or clone this repo on GitHub
2. Go to repo **Settings → Pages → Source: GitHub Actions → Save**
3. Push any change to `main` → GitHub Actions deploys automatically
4. Your app URL will be: `https://YOUR-USERNAME.github.io/REPO-NAME/`

### 📱 Install on iPhone (do this once per device)

1. Open **Safari** on your iPhone
2. Go to your GitHub Pages URL
3. Tap the **Share button** (box with arrow)
4. Tap **"Add to Home Screen"**
5. Tap **"Add"** — done! App icon appears on your home screen

### 🔄 How to update the app

**Option A — Edit on GitHub.com directly:**
1. Open your repo on github.com
2. Click any file → click pencil icon to edit
3. Commit changes → GitHub Actions redeploys in ~60 seconds
4. Open app on iPhone → banner appears "Update available" → tap to refresh

**Option B — Use Claude to update:**
1. Download the file you want to change
2. Ask Claude to make changes (attach the file)
3. Upload the new version back to GitHub
4. GitHub Actions redeploys automatically

**Option C — Claude Code (most powerful):**
1. Open Claude Code in your project folder
2. Ask Claude Code to make any changes
3. Run: `git add . && git commit -m "update" && git push`
4. Done — auto deploys

### 💰 Cost

- **GitHub Pages hosting:** FREE
- **GitHub Actions (deploy automation):** FREE
- **Anthropic API (receipt scanning):** pay per use (~$0.01 per scan)

### 📁 File structure

```
index.html            ← entire app (HTML + CSS + JS)
sw.js                 ← service worker (offline support + update detection)
manifest.json         ← PWA config (icon, colors, display mode)
apple-touch-icon.png  ← iPhone home screen icon (180x180)
icon-192.png          ← PWA icon
icon-512.png          ← PWA icon large
version.txt           ← current version number (bump to trigger update banner)
.github/
  workflows/
    deploy.yml        ← auto-deploy to GitHub Pages on every push
```
