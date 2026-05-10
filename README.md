# caracali-website-vibe-coded

Caracali Open AI Codex site for Webflow. Remote: [github.com/realmzwa/caracali-website-vibe-coded](https://github.com/realmzwa/caracali-website-vibe-coded).

## Git and push from this folder

This directory is already a checkout of [`realmzwa/caracali-website-vibe-coded`](https://github.com/realmzwa/caracali-website-vibe-coded). The `origin` remote uses **SSH**: `git@github.com:realmzwa/caracali-website-vibe-coded.git`.

```bash
cd /Users/mshongwe/Documents/caracali-website-vibe-coded
git status
git push -u origin main
```

Configure your identity if Git asks:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

**Authentication with SSH.** Add an SSH key to your GitHub account ([docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)) so `git push` works without a PAT. Test with `ssh -T git@github.com`. Alternatively you can push from Cursor’s Git panel if signed in there.

### If `/usr/bin/git` fails (`xcrun` / Xcode Command Line Tools)

Install tools with `xcode-select --install`, or temporarily use Git from Miniconda (already installed under `$HOME/miniconda3` on this Mac):

```bash
export PATH="$HOME/miniconda3/bin:$PATH"
git --version
```

Add that `export PATH=...` line to `~/.zshrc` or `~/.bash_profile` if you want it in every Terminal session.

### If Terminal says “could not read Username for 'https://github.com'“

HTTPS needs credentials in a context that can prompt or read stored credentials—use PAT/SSH above, Cursor’s Git panel, or a credential helper.

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
