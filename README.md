# caracali-website-vibe-coded

Caracali Open AI Codex site for Webflow. Remote: [github.com/realmzwa/caracali-website-vibe-coded](https://github.com/realmzwa/caracali-website-vibe-coded).

## Push from this folder

If `git` fails with an Xcode / `xcrun` error, install or repair Apple Command Line Tools (macOS): open Terminal and run `xcode-select --install`, or download “Command Line Tools for Xcode” from Apple’s developer downloads. After `git --version` works:

```bash
cd /Users/mshongwe/Documents/caracali-website-vibe-coded
git init
git remote add origin https://github.com/realmzwa/caracali-website-vibe-coded.git
git branch -M main
git add .
git commit -m "Initial commit"
git push -u origin main
```

SSH remote (if you use SSH keys with GitHub):

```bash
git remote add origin git@github.com:realmzwa/caracali-website-vibe-coded.git
```

Set your identity once (use your GitHub email or noreply):

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Authentication: GitHub no longer accepts account passwords for Git; use a [Personal Access Token](https://github.com/settings/tokens) with HTTPS, or SSH keys.

## Local preview

Open `index.html` in a browser, or use any static server you prefer.

## Deploy on Vercel

The repo is a **static HTML/CSS** site (`index.html` at the repo root). Vercel will serve those files directly.

### From the Vercel dashboard (recommended)

1. Sign in at [vercel.com](https://vercel.com) and click **Add New… → Project**.
2. **Import** [realmzwa/caracali-website-vibe-coded](https://github.com/realmzwa/caracali-website-vibe-coded) from GitHub (install the GitHub integration if prompted).
3. Framework preset: **Other**. Leave **Root Directory** as `./` (default).
4. **Build Command:** leave empty. **Output Directory:** leave empty (or `.` — Vercel uses the repo root).
5. Deploy. Every push to the connected branch will produce a new production deployment (depending on your Vercel project settings).

Production URL appears on the project’s **Deployments** tab; assign a **custom domain** under **Project → Settings → Domains** when you’re ready.

### From the CLI (optional)

Install the [Vercel CLI](https://vercel.com/docs/cli/installation), run `vercel login`, then from this folder:

```bash
cd /Users/mshongwe/Documents/caracali-website-vibe-coded
vercel link
vercel deploy --prod
```

The CLI writes a local `.vercel/` directory with project metadata; it is listed in `.gitignore` so it is not pushed to GitHub.
