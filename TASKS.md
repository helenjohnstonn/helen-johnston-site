# Tasks

Working task list for the site. Everything should ladder up to [GOALS.md](GOALS.md): *a site good enough to send to people and impress them.*

Sections: **Now** (actively building) · **Next** (queued, ready to pick up) · **Later** (someday/ideas) · **Done** (shipped).

---

## Now

- [ ] **Deploy to a custom domain via GitHub Pages.** Decision made: custom domain (most impressive to send). Sub-steps:
  - [ ] Merge `rework-b-side-tracklist` → `main` (latest B-side work; this is what goes live)
  - [ ] Enable GitHub Pages serving from `main` / root → gives a live free `*.github.io` URL immediately
  - [ ] **[Helen]** Pick + register a domain at a registrar (Cloudflare / Namecheap / Porkbun). ~$10-15/yr. This is the only gating step I can't do.
  - [ ] Point the domain's DNS at GitHub Pages + add it as the custom domain in repo settings (I'll give exact records)
  - [ ] Enable "Enforce HTTPS" once the cert provisions
  - [ ] Repoint the Desktop/Dock shortcut at the live custom-domain URL

## Next

- [ ] **Desktop/Dock shortcut** to open the live site in one click (currently points at the local file — update to the live URL once deployed).
- [ ] **Design pass** — Helen has specific design ideas to work through (TBD; capture them here as they come up).
- [ ] **Mobile check** — confirm hero / A Side / B Side / contact all look intentional on a phone.

## Later

- [ ] Custom domain (e.g. helenjohnston.com) if not done at deploy time
- [ ] Performance pass — the repo has several large multi-MB images; compress/resize for fast load
- [ ] Meta tags / link preview (Open Graph image + description) so the link looks good when sent in a message or posted
- [ ] Favicon

## Done

- [x] Bio reworked: leads with core PMM role on YouTube Culture & Artists + YouTube Recap, warmer creative closer (2026-07-07)
- [x] B Side reworked into a creative tracklist; The Wall replaced with contact (2026-06-23)
- [x] B Side built out as zine collage of DJ mixes
- [x] Core sections in place: hero, about, A Side (projects), B Side (creative), contact

---

*How we use this: when you ask "what's next," I'll pull from **Now** → **Next**. When something ships, it moves to **Done** with a date. New ideas land in **Later** so they're not lost.*
