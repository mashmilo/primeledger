# PrimeLedger – deploy guide
1. Create a GitHub repo, upload everything in this folder (keep `settings.json`, `posts/`, `pages/`, `assets/`, `admin/`, `build.js`).
2. Cloudflare Pages → Connect to Git → Build command `node build.js`, Output directory `dist`, env var `NODE_VERSION=20`.
3. Edit `settings.json` → `url` to your real domain (or *.pages.dev URL). Add custom domain later.
4. GitHub → Settings → Developer settings → Fine-grained token: only this repo, Contents = Read & write. Open `yoursite/admin/`, enter `user/repo`, branch, token.
5. Add posts: use the "AI post prompt" tab, ask Claude, paste result, Publish. Cloudflare rebuilds automatically.
6. After AdSense approval: Admin → Theme & Ads → paste `ca-pub-…` and slot IDs. `ads.txt` is generated automatically.
7. Submit `/sitemap.xml` in Google Search Console and Bing Webmaster Tools.
