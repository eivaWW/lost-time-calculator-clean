# Webware — Lost-time cost calculator

A single, self-contained page (`index.html`). No build step, no dependencies. ET/EN toggle. Grounded in McKinsey's ~20%-of-the-workweek benchmark; figures are illustrative.

## Share it — three ways, easiest first

1. **Just send the file (internal / quick).** Send `index.html` to a colleague — they double-click and it opens in any browser. It's fully self-contained.
2. **Public link (best for prospects).** Deploy to Vercel (below) → get a URL like `lost-time-calculator.vercel.app` you can paste into an email.
3. **Embed on the website.** Once it's on Vercel, drop it into a page with an `<iframe src="https://…vercel.app">`.

## Deploy: GitHub → Vercel

You have both accounts. This folder is already a git repo with one commit, so you only push and import.

### Option A — dashboard, no terminal
1. On **github.com** → *New repository* → name it e.g. `lost-time-calculator` → *Create*.
2. *Add file → Upload files* → drag in `index.html` (and this `README.md`) → *Commit*.
3. On **vercel.com** → *Add New → Project* → *Import* that repo → *Deploy*. No settings needed — it's a static site.
4. Vercel returns a public URL. That's your shareable link.

### Option B — terminal (this folder is ready)
```bash
# from this folder
rm -f .git/*.lock .git/objects/*.lock   # one-time: clears leftover setup locks
git remote add origin https://github.com/<your-username>/lost-time-calculator.git
git push -u origin main

npx vercel          # log in, accept defaults → preview URL
npx vercel --prod   # promote to the production URL you share
```

## Update it later
Edit `index.html`, then commit + push (or re-upload the file). Vercel redeploys automatically.

## Custom domain (optional)
Vercel → Project → *Settings → Domains* → add e.g. `kalkulaator.webware.eu` (add the DNS record Vercel shows).

## Honesty notes (keep these true)
- McKinsey's ~20% / ~1.8 h/day is an **external benchmark** — verify before quoting in a proposal.
- The euro figures are an **illustrative model**, not a measured client result.
- Real recoverable time is only known by measuring (a before/after pilot).
