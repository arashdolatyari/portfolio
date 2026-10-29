# Arash Dolatyari Portfolio

A single-page portfolio. No build step: everything lives in `index.html`.

## Edit content
Open `index.html` and look for the block marked **EDIT YOUR CONTENT HERE**:
- `PROFILE`: email, phone, LinkedIn, Dribbble, Medium
- `EXPERIENCE`: places you've worked
- `PROJECTS`: case studies (images go in `assets/projects/`)
- `EXPLORATIONS`: UI explorations

## Add company logos
Put each logo in `assets/logos/`, named after the `slug` in `EXPERIENCE`:
`doctorpay.svg`, `synthetic-solutions.svg`, `jargeh.svg`, `revive-design-lab.svg`,
`mcihub.svg`, `freelance.svg`, `rsimu.svg` (`.png`, `.jpg`, `.webp` also work).
Missing logos show the company's first letter instead.

## Your photo
The hero photo is `assets/arash.jpg`. Replace the file (same name) to change it.

## Project images
Each project has its own folder in `assets/projects/`. An image slot stays hidden until its file exists,
so the live site never shows an empty placeholder. Drop a file in with the right name and it appears.

- `assets/projects/ai-home-design/`: `cover.jpg`, `problem.jpg`, `ia.jpg`, `landing.jpg`, `pricing.jpg`,
  `impact.jpg` (all in place). Empty slot: `findings.jpg`
- `assets/projects/golet/`: `cover.jpg`, `analysis.jpg`, `flow.jpg`, `results.jpg` (all in place).
  Empty slot: `banner.jpg`
- `assets/projects/sunflower/`: `cover.jpg`, `community.jpg`, `paywall.jpg`, `letter.jpg`, `live-groups.jpg`,
  `identity.jpg` (all in place). Empty slots: `onboarding.jpg`, `breathing.jpg`, `progress.jpg`

Case study images are 16:9 (2400×1350 works well). Covers are 2:1 (2400×1200): the same image is the
case study cover and the preview that opens over the project's row on the home page.

Case study pages are in `projects/`. To add a project to the home page, add it to `PROJECTS` in `index.html`.

## UI explorations
Dribbble shots in a row that scrolls sideways, ending with a "See more on Dribbble" button.
Images are 4:3 in `assets/explorations/` (01.jpg, 02.jpg, ...); edit titles in `EXPLORATIONS` in `index.html`.
Clicking an image opens it larger.

## Logos and resume
Company logos are square images in `assets/logos/`, named after each company's `slug` in `EXPERIENCE`
(for example `jargeh.png`). A company without a logo shows its first letter.
The "Resume" link in the menu downloads `assets/Arash_Dolatyari_Product_Designer.pdf`. To update it,
replace that file and keep the same name.

## About page
Edit `about.html`: the title, subtitle, and the `GAMES`, `MOVIES`, and `BOOKS` lists.
Covers go in `assets/about/`, named after the title in lowercase with dashes, for example:
`spec-ops-the-line.jpg`, `call-of-duty-2.jpg`, `call-of-duty-world-at-war.jpg`,
`assassin-s-creed-iv-black-flag.jpg`, `hitman-absolution.jpg`, `ea-sports-fc-fifa-series.jpg`,
`tomb-raider.jpg`, `the-gambler.jpg`, `the-dream-of-a-ridiculous-man.jpg`, `scattered-minds.jpg`,
`the-design-of-everyday-things.jpg`, `the-subtle-art-of-not-giving-a-f-ck.jpg`.
Until a cover is added, a simple title card is shown. The Movies section stays hidden until you add a movie.

## Publish on GitHub Pages
1. Create a new repository on GitHub, for example `portfolio`
   (or `<your-username>.github.io` to get the shortest URL).
2. Upload everything in this folder (Add file → Upload files), then Commit.
3. Go to Settings → Pages. Under "Build and deployment", choose
   Source: Deploy from a branch, Branch: `main`, folder `/ (root)`, then Save.
4. After a minute or two the site is live at
   `https://<your-username>.github.io/portfolio/`.

## Use your own domain later
1. Buy a domain (for example `arashdolatyari.com`).
2. In Settings → Pages → Custom domain, enter it and Save.
3. At your domain registrar, add DNS records:
   - `A` records for `@` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - a `CNAME` record for `www` pointing to `<your-username>.github.io`
4. Once DNS updates, tick "Enforce HTTPS".
