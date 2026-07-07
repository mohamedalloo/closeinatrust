# CloseInATrust

Flagship landing site for closeinatrust.com — trust/LLC vesting lead generation (DSCR-heavy), an AdaptLend service. Navy/brass identity, RetiredRefi architecture.

Static site: `index.html` + `styles.css` + `script.js`. No build step.

## Lead storage

Form inserts into the shared AdaptLend Supabase `leads` table (insert-only RLS, publishable key in `script.js`). Attribution: `matched_product` suffix `— CloseInATrust`.

## Deploy

Same GitHub Pages pattern: push, enable Pages from `main` root (CNAME in place), Namecheap DNS (4 GitHub A records + www CNAME), Enforce HTTPS. Point satellite domains (closeinanllc.com, buyinatrust.com, llcheloc.com) here with permanent redirects.

## Compliance notes

- Brand of the AdaptLend service (Honest Casa LLC, NMLS #1566096, DRE #02022356). Confirm DBA requirements with counsel.
- Footer carries a "not legal/tax advice" disclaimer for trust/entity content, including the Garn-St Germain references — keep it.
- No welcome email wired; success screen mentions email — wire or soften before heavy traffic.
