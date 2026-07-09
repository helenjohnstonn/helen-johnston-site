# Tasks

Working task list for the site. Everything should ladder up to [GOALS.md](GOALS.md): *a site good enough to send to people and impress them.*

Sections: **Now** (actively building) · **Next** (queued, ready to pick up) · **Later** (someday/ideas) · **Done** (shipped).

---

## Now

- [ ] **Handwriting follow-ups** (reminder scheduled for 2026-07-08 9am):
  - [ ] Commit the handwriting work (currently uncommitted on worktree branch `claude/vigorous-shtern-78a9da`) + PR to main
  - [x] ~~Remove the A-Side / B-Side discipline labels from the bio~~ — done 2026-07-07, whole disciplines block (labels + subgenre tags) deleted
  - [x] ~~Prototype the A Side / B Side section headers in the handwritten assets~~ — done 2026-07-07: both headers converted (mask + `currentColor`, sized up to 1.25em), correct on both sides of the flip
- [ ] **Deploy to a custom domain via GitHub Pages.** Decision made: custom domain (most impressive to send). Remaining sub-steps:
  - [ ] **[Helen]** Pick + register a domain at a registrar (Cloudflare / Namecheap / Porkbun). ~$10-15/yr. This is the only gating step Helen has to do herself.
  - [ ] Point the domain's DNS at GitHub Pages + add it as the custom domain in repo settings (Claude will give exact records)
  - [ ] Enable "Enforce HTTPS" once the cert provisions
  - [ ] Repoint the Desktop/Dock shortcut at the live custom-domain URL

## Next

- [ ] **Add real B-side assets.** The strip is now Graphic Design (was Photography, changed 2026-07-07) and shows 1 real image (the djing sketch) + "+ Design" placeholders. Helen to select/export posters/layouts/identity work ("plenty but not ready").
- [ ] **A-side redesign — undecided.** Helen may want to rethink the A-side (product work) so it stops feeling like a visual resume, but not yet. Revisit after B-side settles.
- [ ] **Desktop/Dock shortcut** to open the live site in one click (currently points at the local file — update to the live URL once deployed).
- [ ] **Design pass** — Helen has specific design ideas to work through (TBD; capture them here as they come up).

## Later

- [ ] **More handwritten elements** — hero nav, top nav, and the bio name are now real handwriting (see Done). Remaining candidates: the A-Side/B-Side discipline labels in the about section, the contact headline, "Flip to B-Side" fab. Same pipeline: Helen writes it, photo → masked WebP asset.
- [ ] Meta tags / link preview (Open Graph image + description) so the link looks good when sent in a message or posted
- [ ] Favicon
- [ ] Mobile hero: nav labels ("A Side" / "B Side") slightly overlap the HELEN wordmark — reads as zine-collage, but worth a deliberate look during the design pass

## Done

- [x] **Real handwriting everywhere the site faked it** — hero canvas nav (About/A-Side/B-Side/Contact, rotated right-edge on desktop, horizontal A/B on mobile), top nav links, and the bio "Helen Johnston" (two photos composed into one baseline-aligned lockup) are all Helen's actual marker lettering; masked WebP assets follow the theme color on both sides; hit areas track the drawn art (2026-07-07)
- [x] **Fixed latent hero-death bug** — loading the site in a hidden/background tab killed the hero canvas draw loop permanently (0-size canvas threw mid-frame); now it bails and self-heals when the tab becomes visible (2026-07-07)
- [x] Handwritten "HELEN" in the bio — first pass of the handwriting pipeline, superseded same day by the full name lockup (2026-07-07)
- [x] Bio reworked: leads with core PMM role on YouTube Culture & Artists + YouTube Recap, warmer creative closer (2026-07-07)
- [x] **Real SoundCloud audio wired into the B-side player** — hidden Widget API embed drives the custom UI; all 3 real mixes (Mean Gills Y2K / Magical Forest / UKG Prescription) with true durations, play/pause/seek/track-switch verified (2026-07-07)
- [x] **Contact section redone neo-brutalist** — marquee ticker, hard-shadow slab links with hover invert, rubber-stamp badge, barcode colophon; inverts with the A/B flip; verified desktop + mobile (2026-07-07)
- [x] Mobile hero nav fixed — A/B Side below the wordmark, About/Contact dropped on mobile; hero labels trigger the flip (2026-07-07)
- [x] Record flip + music-first B-side actually merged to main (was stranded on an unmerged branch) via PR #7 (2026-07-06)
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
