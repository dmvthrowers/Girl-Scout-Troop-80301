# Troop 80301 website — deploy notes

Everything in this folder goes into https://github.com/dmvthrowers/Girl-Scout-Troop-80301
(the repo is empty right now except LICENSE + README).

## Deploy (5 minutes)

1. Open the repo on GitHub → **Add file → Upload files** → drag in everything
   from this folder. (The repo's README.md will be replaced by the template's —
   that's fine, or keep yours and skip that one file.)
2. **Settings → Pages → Build and deployment → Source → GitHub Actions.**
3. Push to `main` (or it deploys on the upload). Wait ~1–2 minutes.
4. Live at `https://dmvthrowers.github.io/Girl-Scout-Troop-80301/`

Or hand this folder to Claude Code — the template's AGENTS.md/CLAUDE.md tell it
exactly what to do.

## What's filled in (from Heather's emails)

- Troop 80301, Dumfries VA, founded 2026, multi-level K–5, Covington-Harper ES
- Council: Girl Scouts Nation's Capital, Service Unit 80-4
- Events: SU 80-4 meeting Oct 13, 2026; first troop meeting TBA
- Girl Scout green/gold theme, Daisy→Ambassador levels page, safety/privacy pages

## Still TODO (marked in site.jsonc too)

- [ ] **Troop email** — set up a shared address (not a personal one) in `contact.email`
- [ ] **Meeting time/location** — was undecided as of Sep 29; update `meetings`
- [ ] **Leaders** — Heather, Jazmine, Kathleen aren't named until each says yes
      (public site, kids' troop — get explicit consent first)
- [ ] **Dues** — currently "To be announced"
- [ ] Photos — only with written parent permission, no full names of girls
