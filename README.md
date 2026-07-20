# CatilizeZero

Coming-soon landing page for **catilizezero.com** — the Catilize®Zero™ Foundation, from Catilize Health.

The whole site is the single `index.html` (no build step; the only external request is Google Fonts for Source Sans 3). Deploy by uploading `index.html` as the document root of catilizezero.com on any static host.

Design follows the Catilize Branding Guide (CAT-0002, Feb 2021): brand purple `#420098`, magenta `#E030F3` / cyan `#26FFE8` accents, master color blend background, C-ring logo motif, Source Sans Pro (Source Sans 3) type.

## Adding the HubSpot form

1. In `index.html`, find the `HUBSPOT FORM EMBED` comment inside `<div id="hubspot-form">`.
2. Paste the HubSpot embed code below the comment.
3. Delete the fallback block between `FALLBACK START` and `FALLBACK END`.
4. Redeploy.

The page ships with CSS for HubSpot's form classes (`.hs-form`, `.hs-input`, `.hs-button`, error/success states), so a standard inline embed styles itself to the brand. If the portal forces an iframe embed, style the form in HubSpot's form editor instead (button `#E030F3`, labels `#FBFAFF`).

## Related

- Sister site: [CatilizeRx](https://github.com/anneallen/CatilizeRx) (catilizerx.com)
- catilize-rx.com should 301-redirect at the host/DNS level (confirm target: catilizerx.com vs catilizezero.com).
