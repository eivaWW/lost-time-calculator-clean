# Webware — Lost-time calculator (clean / minimal variant)

The **minimal** sibling of `lost-time-calculator`. Same inputs, same maths, same honesty — but numbers-first: the two euro figures are front and centre, and everything else (the working-week view, the "1 document → process points" visual, the before/after table, the sources) sits behind click-to-open rows. Built for a C-level glance.

Single self-contained `index.html`, no build step, ET/EN toggle.

## Why two versions
This exists to A/B against the richer `lost-time-calculator`:
- **Rich version** — tells the whole story on one page (more scrolling, more to read, more persuasive in a guided demo).
- **Clean version (this)** — answer in 3 seconds, detail on demand (better for sending a link to a busy executive).

## Share / deploy — GitHub → Vercel (separate project)
Deploy this as its **own** Vercel project so both live side by side.
1. github.com → **New repository** → name e.g. `lost-time-calculator-clean` → Create.
2. **Add file → Upload files** → drag `index.html` (and this `README.md`) → Commit.
   - Or terminal: `rm -f .git/*.lock .git/objects/*.lock` then `git remote add origin https://github.com/<you>/lost-time-calculator-clean.git` → `git push -u origin main`.
3. vercel.com → **Add New → Project** → import the repo → **Deploy**. You'll get a second URL to compare against the rich one.

## Honesty notes (same as the rich version)
- Search-time 20–30%: McKinsey / IDC / Forrester — external, verify before a proposal.
- Euro figures and the reclaimable share are an **illustrative model**, confirmed by a pilot.
- Employer-tax multiplier (~1.34) is Estonia-specific.
