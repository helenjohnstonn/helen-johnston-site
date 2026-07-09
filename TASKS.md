# Tasks

Working task list for the site. Everything should ladder up to [GOALS.md](GOALS.md): *a site good enough to send to people and impress them.*

Sections: **Now** (actively building) · **Next** (queued, ready to pick up) · **Later** (someday/ideas) · **Done** (shipped).

---

## Now

- [ ] **Deploy to a custom domain via GitHub Pages.** Live at itsjusthel.com over HTTP (2026-07-09) — Helen registered the domain, set the DNS A/CNAME records, and added it in repo settings herself. Remaining:
  - [ ] Enable "Enforce HTTPS" once GitHub's cert provisions (was still provisioning as of 2026-07-09 afternoon; usually minutes-to-hours)
  - [ ] Repoint the Desktop/Dock shortcut at https://itsjusthel.com

## Next

- [ ] **Expandable graphic design pieces** — clicking a design in the B-side graphic design strip should expand it (lightbox/full-size view).
- [ ] **B-side text color fix** — after flipping to the B side, A-side section text (e.g. "Find Hub") should be black, not white.
- [ ] **A-side redesign — undecided.** Helen may want to rethink the A-side (product work) so it stops feeling like a visual resume, but not yet. Revisit after B-side settles.
- [ ] **Desktop/Dock shortcut** to open the live site in one click (currently points at the local file — update to the live URL once deployed).
- [ ] **Design pass** — Helen has specific design ideas to work through (TBD; capture them here as they come up).

## Later

- [ ] **More handwritten elements** — hero nav, top nav, and the bio name are now real handwriting (see Done). Remaining candidates: the A-Side/B-Side discipline labels in the about section, the contact headline, "Flip to B-Side" fab. Same pipeline: Helen writes it, photo → masked WebP asset.
- [ ] Meta tags / link preview (Open Graph image + description) so the link looks good when sent in a message or posted
- [ ] Favicon
- [ ] Mobile hero: nav labels ("A Side" / "B Side") slightly overlap the HELEN wordmark — reads as zine-collage, but worth a deliberate look during the design pass

## Done

- [x] **Hero record interactive works on mobile** — mouse-only listeners swapped for pointer events (mouse + touch + pen) so touch drags/presses drive the warp; `touch-action: pan-y pinch-zoom` keeps vertical swipes scrolling the page; verified in preview at 375px, desktop behavior unchanged (2026-07-09)
- [x] **Contact channel slabs made playful** — email updated to helensjohnston@gmail.com; each of the four links now has its own zine-sticker colour (orange/teal/mustard/pink), a taped-on tilt that straightens + floods with its colour on hover, an in-voice caption line ("for the important stuff", "the professional one", "hear me mix", "photos + chaos"), and A1/A2/B1/B2 catalog numbers; tilt neutralised on mobile (2026-07-09)
- [x] **Bio rewritten** — Helen's updated three-paragraph bio (Core & Artists team, builder-at-heart framing, "little corner of the internet" closer); name handwriting asset preserved as the opener (2026-07-09)
- [x] **B-side polish pass merged to main** via PR #20 — waveform pulses with playback (synthesized groove; SC iframe is cross-origin so no real FFT), Graphic Design heading enlarged w/ orange offset-print layer, real SoundCloud cover art on the record label, and all 10 real designs from Helen's "Graphic Design" folder in the strip as free-width 430px-tall WebPs (~270KB total; old djing-sketch2.webp removed) (2026-07-09)
- [x] **Handwriting branch merged to main** via PR #19 — all real-handwriting work + hidden-tab hero fix now live (2026-07-08)
- [x] **Real handwriting everywhere the site faked it** — hero canvas nav (About/A-Side/B-Side/Contact, rotated right-edge on desktop, horizontal A/B on mobile), top nav links, section headers, and the bio "Helen Johnston" (two photos composed into one baseline-aligned lockup) are all Helen's actual marker lettering; masked WebP assets follow the theme color on both sides; hit areas track the drawn art; bio discipline labels/tags removed (2026-07-07)
- [x] **Fixed latent hero-death bug** — loading the site in a hidden/background tab killed the hero canvas draw loop permanently (0-size canvas threw mid-frame); now it bails and self-heals when the tab becomes visible (2026-07-07)
- [x] Handwritten "HELEN" in the bio — first pass of the handwriting pipeline, superseded same day by the full name lockup (2026-07-07)
- [x] **Custom pointer-finger cursor** — Helen's halftone hand image (Desktop `PointerFinger.jpg`) cut out to a transparent PNG and used as the cursor site-wide (64px + retina 2x via image-set; default, links/buttons, hero canvas); the old orange cursor-ring follower removed in favor of the hand (2026-07-08)
- [x] **Hero fixed on wide screens** — wordmark size now clamped by viewport height (was width-only, so wide/short laptop windows clipped HELEN off-screen); right-edge nav labels scale up on tall screens (2026-07-07)
- [x] **Scroll reveals made resilient** — sections no longer hidden by CSS awaiting GSAP; hidden state applied via gsap.set so content stays visible if the CDN is blocked (verified with GSAP disabled) (2026-07-07)
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
