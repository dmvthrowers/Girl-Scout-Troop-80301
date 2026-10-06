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
