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

- [ ] **Wire real audio into the B-side player.** Player UI is built but playback is *simulated* (timeline + waveform animate). Needs final SoundCloud track URLs, then hook up the SoundCloud Widget API for live audio. (Decision made: persistent player with real audio.)
- [ ] **Add real B-side assets.** Photography strip currently shows 2 real images + placeholders; graphic design not yet surfaced. Helen to select/export work ("plenty but not ready").
- [ ] **A-side redesign — undecided.** Helen may want to rethink the A-side (product work) so it stops feeling like a visual resume, but not yet. Revisit after B-side settles.
- [ ] **Desktop/Dock shortcut** to open the live site in one click (currently points at the local file — update to the live URL once deployed).
- [ ] **Mobile check** — confirm hero / A Side / B Side / contact all look intentional on a phone (player goes single-column < 768px).

## Later

- [ ] Custom domain (e.g. helenjohnston.com) if not done at deploy time
- [ ] Performance pass — the repo has several large multi-MB images; compress/resize for fast load
- [ ] Meta tags / link preview (Open Graph image + description) so the link looks good when sent in a message or posted
- [ ] Favicon

## Done

- [x] **B Side redesigned music-first** — flat B1/B2/B3 tracklist replaced with a featured "Now Spinning" player (disc = play button, animated waveform/scrubber, transport), a set list of mixes, and a photography filmstrip (2026-06-23)
- [x] **Record flip made real** — the dead flip code now works: a flip button (+ A/B nav links) spins a record and inverts the whole site between the A-side (orange/professional) and B-side (teal/creative) palettes; deep-link `#creative` lands on the B-side (2026-06-23)
- [x] Hero kept as-is (the warped "HELEN" vinyl) — confirmed it's the anchor, not to be touched (2026-06-23)
- [x] B Side reworked into a creative tracklist; The Wall replaced with contact (2026-06-23)
- [x] B Side built out as zine collage of DJ mixes
- [x] Core sections in place: hero, about, A Side (projects), B Side (creative), contact

---

*How we use this: when you ask "what's next," I'll pull from **Now** → **Next**. When something ships, it moves to **Done** with a date. New ideas land in **Later** so they're not lost.*
