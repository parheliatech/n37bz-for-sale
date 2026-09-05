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

Open a terminal **on your own computer**, `cd` into this folder, then:

```bash
git init
git add .
git commit -m "Initial N37BZ for-sale site"
```

Then, on github.com (you're logged in as parheliatech):
1. Click **New repository**. Suggested name: `n37bz-for-sale`
   (public, so GitHub Pages can serve it for free; don't initialize it
   with a README/license — this folder already has one).
2. Copy the commands GitHub shows under "…or push an existing repository
   from the command line", e.g.:

```bash
git remote add origin https://github.com/parheliatech/n37bz-for-sale.git
git branch -M main
git push -u origin main
```

3. In the new repo on GitHub: **Settings → Pages** → under "Build and
   deployment", set **Source** to "Deploy from a branch", branch `main`,
   folder `/ (root)`, then **Save**.
4. GitHub will give you a live URL, typically:
   `https://parheliatech.github.io/n37bz-for-sale/`
   (takes a minute or two to go live after the first push).

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
