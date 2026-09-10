# sori-site

Public pages for the Sori app (Korean learning from short clips of Korean
shows), served by GitHub Pages at https://adidasneumann-glitch.github.io/sori-site/:

- `privacy.html` — privacy policy (GDPR; controller = the publisher, an individual in the Czech Republic)
- `terms.html` — terms of use, including the Sori Pro subscription terms
- `support.html` — support page and FAQ
- `index.html` — landing page linking the three

Plain static HTML, no build step, no analytics, no cookies. `.nojekyll` keeps
GitHub from running Jekyll over the files.

The app repo (private) reads the privacy and terms URLs from
`src/features/entitlements/purchases/config.ts`; the same URLs go into App
Store Connect and Play Console. Each page carries a version and an effective
date in its header: bump both when the text changes.
