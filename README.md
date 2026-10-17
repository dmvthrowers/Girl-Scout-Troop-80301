# Girl Scout Troop 80301 Website

The website for Girl Scout Troop 80301 (Dumfries, Virginia). It's live at
**https://dmvthrowers.club/Girl-Scout-Troop-80301/**.

DMV Throwers volunteers maintain it. It is built from the free
[Scouts Template Site](https://github.com/dmvthrowers/Scouts-Template-Site): you edit one settings
file and GitHub builds and publishes the site. No cookies, trackers, or outside fonts.

## Update the site

1. Open [`site.jsonc`](site.jsonc) on GitHub and click the pencil icon.
2. Change the text you need (meeting time, events, contact, leaders). Every setting has a comment.
3. Commit. GitHub builds and publishes the site in 1 to 2 minutes.

Only list a leader or show a photo with their or a parent's written OK.

To preview on your computer: `python3 build.py && python3 scripts/check_site.py`, then open
`_site/index.html`. The check catches broken links, empty email links, and accessibility mistakes.

## Events from Google Calendar (optional)

The site can list upcoming events from the troop's Google Calendar on its own, every morning, with times.

1. In Google Calendar, open the calendar's **Settings and sharing > Integrate calendar** and copy the
   **Secret address in iCal format**. It works even if the calendar is private. Treat it like a password.
2. In this repository: **Settings > Secrets and variables > Actions > New repository secret**. Name it
   `CALENDAR_ICS_URL` and paste the address. Optional, on the **Variables** tab: `CALENDAR_TZ` = `America/New_York`.
3. **Actions > Build and deploy > Run workflow**. After that, changes to the calendar show up within a day.

Only each event's title, date, time and place are used, and places stay hidden unless `"show_places": true` is set
under `calendar` in `site.jsonc`. A description stays on the calendar unless it starts with `Public:`. Private and
cancelled events are skipped. An event in `site.jsonc` replaces calendar events on the same day. With no secret, the
site builds from `site.jsonc` as before.

## Pull in template updates

```
git remote add upstream https://github.com/dmvthrowers/Scouts-Template-Site.git
git fetch upstream
git merge upstream/main
python3 build.py && python3 scripts/check_site.py
```

Keep your own `site.jsonc` when resolving conflicts.

## Notes

- [`DEPLOY.md`](DEPLOY.md) lists what is still to do.
- [`TEMPLATE-README.md`](TEMPLATE-README.md) is the full template guide (presets, custom domain, calendar).
- [`SECURITY.md`](SECURITY.md) explains how to report a problem.
- License: [Unlicense](LICENSE), public domain.
