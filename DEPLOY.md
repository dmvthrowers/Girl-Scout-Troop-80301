# Troop 80301 website: maintenance notes

The site builds with GitHub Actions and publishes to
https://dmvthrowers.club/Girl-Scout-Troop-80301/ (see README for how to edit it).

## What's filled in

- Troop 80301, Dumfries VA, founded 2026, multi-level K-5, Covington-Harper ES
- Council: Girl Scouts Nation's Capital, Service Unit 80-4
- Events: SU 80-4 meeting Oct 13, 2026; first troop meeting TBA
- Girl Scout green/gold theme, Daisy to Ambassador levels page, safety and privacy pages

## Still to do (also marked in site.jsonc)

- [ ] **Troop email**: set up a shared address (not a personal one) in `contact.email`.
      Until then the site points visitors to the contact page.
- [ ] **Meeting time and location**: update `meetings` once decided.
- [ ] **Leaders**: list a person only after they say yes (public site, kids' troop).
- [ ] **Dues**: currently "To be announced".
- [ ] **Photos**: only with written parent permission, no full names of girls.
- [ ] **Own domain (optional)**: the site lives at the URL above for now. For a domain like
      `troop80301.org` (about $10-20/yr; check the renewal price and ask GSCNC before using
      "girlscouts" in the name), follow README, "Custom domain".
