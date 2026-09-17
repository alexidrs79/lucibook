# lucibook

Landing-page theme for **Lucibook**, the workspace that ties Snap (document capture), LuciCore (reconciliation), and Luci AI together. Live at `lucibook.co.uk`.

A field group per section in `inc/`, a part per section in `template-parts/`, and the `Lucibook Landing` page template pulling them in order — Hero, Social Proof, Reconciliation, Luci AI, One Connected Workspace, Pricing, Founding Offer.

- Built from Figma node `15532:79` ("Lucibook — Final Landing Page"), with the design tokens at the top of `style.css` taken from that file rather than eyeballed.
- Media lookups use the filename-stem style from the start, so `inc/media-defaults.php` carries no numeric attachment IDs.

## Requirements

- WordPress 6.4 or newer, PHP 8.0 or newer
- Advanced Custom Fields **Pro** — field groups use repeaters and options pages, neither of which the free plugin provides, so a theme activated without it renders its sections empty.

## Installing

Copy or symlink this folder into `wp-content/themes/` and activate it. Create a page and assign the `Lucibook Landing` page template. Section content is then filled in on the page itself, with site-wide values under the theme's own options page.

## Deploys

There is no automated deploy. Code and content go live manually — a change that works locally is not live until it is copied up, and the database side (ACF values, Media Library items) has to be reproduced on the target install by hand. Use the filename-stem media lookups for anything new; a numeric attachment ID only works on the install it was captured against.
