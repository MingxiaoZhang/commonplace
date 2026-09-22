# Setting up The Commonplace in Claude Code + GitHub

This archive unpacks into a complete git repo (history already committed on `main`).

## 1. Unpack and open
    unzip commonplace.zip
    cd commonplace
    git log --oneline          # you should see the initial commit

## 2. Point it at Claude Code
Open this folder in Claude Code (or `claude` from inside it). It's plain
HTML/CSS with no build step, so nothing to install.

## 3. Create the GitHub remote and push
Using the GitHub CLI (easiest — creates the repo and pushes in one step):
    gh repo create commonplace --private --source=. --push

Or manually: create an empty repo on github.com, then:
    git remote add origin git@github.com:YOURNAME/commonplace.git
    git push -u origin main

## 4. (Optional) Publish the site
- **GitHub Pages:** repo Settings > Pages > deploy from `main` / root.
- **Vercel / Cloudflare Pages:** import the repo; framework preset = "Other"
  (no build command, output dir = root).

## Before you go live
- Fill the footer links (email / GitHub / LinkedIn) in `index.html`.
- Set Ambit's "View →" link (currently `#`).
- Set your real git identity (this commit used a placeholder):
      git config user.name  "Your Name"
      git config user.email "you@yourhost.com"
