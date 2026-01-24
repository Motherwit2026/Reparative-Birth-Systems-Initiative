# Reparative Birth Systems Initiative — Website

This repository contains the project for community-governed knowledge & policy infrastructure for birth justice.

How to publish this starter site with GitHub Pages:

Option A — Quick (no build)
1. Add the files `index.html` and `styles.css` to the repository root (or put them in a `docs/` folder).
2. In the repository Settings > Pages:
   - Source: choose branch `main` and select folder `/ (root)` if files are at root, or `/docs` if you placed them there.
   - Save. GitHub will provide a site URL after deployment.
3. If the repo is private, ensure your GitHub plan supports Pages for private repos; otherwise make the repo public or use an external host (Netlify/Vercel).

Option B — Using a static site generator (Jekyll/Hugo/Next)
- Use a generator for multi-page structure, templates, and assets. I can scaffold this if you prefer.

Custom domain
- Add your domain in Settings > Pages > Custom domain and configure DNS (CNAME or A record) as instructed.

Want me to push these starter files into your repo and enable Pages settings (or add a GitHub Actions workflow to deploy automatically)? Reply with what you want:
- "Push files and enable Pages (root)" or
- "Push files into /docs and enable Pages (/docs)" or
- "I want a Next.js site" or
- "Give me steps only"

Publishing notes and choices
- If you want the absolute fastest path: copy these two files (index.html + styles.css) into the repo root, then enable Pages to publish from main /root.
- If you want continuous deployment with changes built (e.g., using a framework), I can scaffold a workflow that builds and deploys via GitHub Actions or recommend Netlify/Vercel for frameworks like Next.js.
- Tell me if you want a custom domain, a specific design or colors, or a content structure (pages: About / Projects / Resources / Contribute) — I’ll adapt the starter site.

What would you like me to do now?
- I can push the starter files and enable Pages for you (I’ll need permission to push or you can accept the PR I create). If you want me to push, confirm "Push to repo and enable Pages (root)" and I’ll create the branch and files for you.