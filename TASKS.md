# Tasks

Working task list for the site. Everything should ladder up to [GOALS.md](GOALS.md): *a site good enough to send to people and impress them.*

Sections: **Now** (actively building) · **Next** (queued, ready to pick up) · **Later** (someday/ideas) · **Done** (shipped).

---

## Now

- [ ] **Deploy to a custom domain via GitHub Pages.** Decision made: custom domain (most impressive to send). Remaining sub-steps:
  - [ ] **[Helen]** Pick + register a domain at a registrar (Cloudflare / Namecheap / Porkbun). ~$10-15/yr. This is the only gating step Helen has to do herself.
  - [ ] Point the domain's DNS at GitHub Pages + add it as the custom domain in repo settings (Claude will give exact records)
  - [ ] Enable "Enforce HTTPS" once the cert provisions
  - [ ] Repoint the Desktop/Dock shortcut at the live custom-domain URL

## Next

- [ ] **Wire real audio into the B-side player.** Player UI is built but playback is *simulated* (timeline + waveform animate). Needs final SoundCloud track URLs, then hook up the SoundCloud Widget API for live audio. (Decision made: persistent player with real audio.)
- [ ] **Add real B-side assets.** Photography strip currently shows 2 real images + placeholders; graphic design not yet surfaced. Helen to select/export work ("plenty but not ready").
- [ ] **A-side redesign — undecided.** Helen may want to rethink the A-side (product work) so it stops feeling like a visual resume, but not yet. Revisit after B-side settles.
- [ ] **Desktop/Dock shortcut** to open the live site in one click (currently points at the local file — update to the live URL once deployed).
- [ ] **Design pass** — Helen has specific design ideas to work through (TBD; capture them here as they come up).

## Later

- [ ] Meta tags / link preview (Open Graph image + description) so the link looks good when sent in a message or posted
- [ ] Favicon
- [ ] Mobile hero: nav labels ("A Side" / "B Side") slightly overlap the HELEN wordmark — reads as zine-collage, but worth a deliberate look during the design pass

## Done

- [x] Performance pass — converted all images to right-sized WebP (~20MB → 1.3MB), removed 2 unused images (2026-07-06)
- [x] Mobile check — hero / about / A Side / B Side / contact verified at 375px, no overflow, all images load (2026-07-06)
- [x] GitHub Pages enabled, serving `main` — live at https://helenjohnstonn.github.io/helen-johnston-site/ (repo made public; history scanned for secrets first — clean) (2026-07-06)
- [x] `rework-b-side-tracklist` merged to `main` via PR #3 (2026-07-06)
- [x] **B Side redesigned music-first** — flat B1/B2/B3 tracklist replaced with a featured "Now Spinning" player (disc = play button, animated waveform/scrubber, transport), a set list of mixes, and a photography filmstrip (2026-06-23, merged to main 2026-07-06)
- [x] **Record flip made real** — the dead flip code now works: a flip button (+ A/B nav links) spins a record and inverts the whole site between the A-side (orange/professional) and B-side (teal/creative) palettes; deep-link `#creative` lands on the B-side (2026-06-23, merged to main 2026-07-06)
- [x] Hero kept as-is (the warped "HELEN" vinyl) — confirmed it's the anchor, not to be touched (2026-06-23)
- [x] B Side reworked into a creative tracklist; The Wall replaced with contact (2026-06-23)
- [x] B Side built out as zine collage of DJ mixes
- [x] Core sections in place: hero, about, A Side (projects), B Side (creative), contact

---

*How we use this: when you ask "what's next," I'll pull from **Now** → **Next**. When something ships, it moves to **Done** with a date. New ideas land in **Later** so they're not lost.*
