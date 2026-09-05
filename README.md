# N37BZ VariEze — For Sale site

This folder is a ready-to-publish GitHub Pages site for selling N37BZ.

## What's here
- `index.html` — the whole site (single file, no build step)
- `images/` — 24 web-optimized photos (resized/compressed from your originals)
- `logbooks/` — compressed engine & airframe logbook PDFs, linked from the page

## Current status
No placeholders remain — the page is ready to publish as-is. It currently
includes: price $32,000, Tucson/KRYN, TTAF 756 hrs / ~30 hrs since the
high-compression C-85 piston & overhauled-cylinder installation, Dynon
EFIS, uAvionix ADS-B in/out, Terra TX-760D com, Terra TRT-250D transponder,
Narco Escort II nav/com w/ glideslope, last condition inspection May 16
2026, the cylinder-paperwork disclosure, a "What's Included" section
(spare prop, new never-installed wheelpants, canopy cover), and a note
that you're willing to fly it to the new owner.

Feel free to still edit wording, swap the hero photo (currently
`images/photo-01.jpg`), reorder the gallery, or add more detail — it's
plain HTML/CSS/JS, easy to hand-edit.

## Publish it to GitHub Pages

### Step 1 — Create the (empty) repository on github.com
1. Go to https://github.com/new (you're logged in as parheliatech).
2. Repository name: `n37bz-for-sale`
3. Set it to **Public** (required for free GitHub Pages).
4. Leave every checkbox unchecked (no README, no .gitignore, no license) —
   this folder already has its own files and adding any of those on
   GitHub's side would conflict with the push in Step 2.
5. Click **Create repository**. You'll land on a mostly-empty page for
   the new repo — you don't need to read or copy anything from it,
   just leave that browser tab open and move to Step 2.

### Step 2 — Push this folder to it
Open a terminal **on your own computer**, `cd` into this exact folder
(the one this README is in), then run these commands exactly as written
(the URL is specific to the repo you just made):

```bash
git init
git add .
git commit -m "Initial N37BZ for-sale site"
git remote add origin https://github.com/parheliatech/n37bz-for-sale.git
git branch -M main
git push -u origin main
```

If it asks you to sign in, follow its prompts (browser login or a
personal access token as the password) — that's GitHub authenticating
you, not something to worry about.

### Step 3 — Turn on Pages
Back in the browser tab from Step 1 (or navigate to
`https://github.com/parheliatech/n37bz-for-sale/settings/pages`):
1. Under **Build and deployment → Source**, choose **Deploy from a branch**.
2. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
3. Wait a minute or two, then refresh that Pages settings page — it will
   show your live URL at the top, which will be:
   `https://parheliatech.github.io/n37bz-for-sale/`

That URL is what you link to from Facebook, Barnstormers, etc.

## Updating later
Whenever you change something in this folder (price, add photos, fix a
typo):

```bash
git add .
git commit -m "Update listing"
git push
```

GitHub Pages redeploys automatically within a minute or two.
