# AMITAI — Carnatic Music Teacher

Your personal Carnatic music teacher. Learn swaras through guided practice, ear training, Sarali Varisai, and an AI guru.

## Deploy to Vercel (2 minutes)

### Option A: Drag & Drop (Easiest)
1. Go to [vercel.com](https://vercel.com) and sign up (free)
2. Click **"Add New" → "Project"**
3. Choose **"Import Third-Party Git Repository"** or simply drag the `amitai-deploy` folder onto the page
4. Click **Deploy**
5. Done! You'll get a URL like `amitai-xxxxx.vercel.app`

### Option B: Via CLI
```bash
npm i -g vercel
cd amitai-deploy
vercel
```
Follow the prompts. Takes 30 seconds.

### Option C: Via GitHub
1. Create a new GitHub repo (e.g., `amitai`)
2. Push this folder to it:
   ```bash
   cd amitai-deploy
   git init
   git add .
   git commit -m "AMITAI v1"
   git remote add origin https://github.com/YOUR_USERNAME/amitai.git
   git push -u origin main
   ```
3. Go to [vercel.com](https://vercel.com) → **Import** → select the repo → **Deploy**
4. Bonus: Every future `git push` auto-deploys

## Custom Domain (Optional)
In Vercel dashboard → Settings → Domains → add `amitai.yourname.com`

## What's Included
- `public/index.html` — The full AMITAI app (single file, no build step)
- `public/manifest.json` — PWA manifest (enables "Add to Home Screen")
- `public/icon-192.png` / `icon-512.png` — App icons
- `vercel.json` — Vercel routing config

## PWA: Add to Home Screen
Once deployed, users on mobile can tap **Share → Add to Home Screen**. The app launches fullscreen with your icon — no browser chrome.

## Note on Amit Mode
Amit Mode (AI guru) calls the Anthropic API. It currently works within Claude's environment but will need an API proxy for production. For v1, the other 3 modes (Raga Practice, Quiz Mode, Varisai Practice) work perfectly without any backend.
