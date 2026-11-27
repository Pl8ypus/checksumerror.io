# checksumerror.io

Static one-page site for Checksum Error. Plain HTML and CSS, no build step. Hosted on GitHub Pages.

## Files
| File | What it is |
|---|---|
| `index.html` | The whole site (CSS inline, ~20 KB) |
| `404.html` | Not-found page |
| `CNAME` | Tells GitHub Pages the custom domain is `checksumerror.io` |
| `.nojekyll` | Stops GitHub Pages running Jekyll on the files |
| `favicon.svg`, `apple-touch-icon.png` | Browser and home-screen icons |
| `og.png` | 1200x630 link-preview image (Instagram bio, iMessage, Slack, X) |
| `robots.txt`, `sitemap.xml` | For search engines |

## Placeholders to replace
Search the repo for `REPLACE_ME`. Every one must be replaced before you share the site.

| Placeholder | Where | Replace with |
|---|---|---|
| `REPLACE_ME_ETSY_SHOP` | hero button, footer, JSON-LD | Your Etsy shop name as in `etsy.com/shop/<name>` |
| `REPLACE_ME_01` … `REPLACE_ME_05` | the 5 "buy on etsy" buttons | Each listing's number from `etsy.com/listing/<number>/...` (01 Works On My Machine, 02 Sudo Make Coffee, 03 Just One More Prompt, 04 Ship It, 05 Human In The Loop) |
| `REPLACE_ME_INSTAGRAM` | Instagram button, footer, JSON-LD | Your Instagram handle. The heading also says `@checksumerror` (a guess): change it if the handle differs |
| `REPLACE_ME_EMAIL_FORM_ACTION` | signup form `action` | Your email provider's form endpoint (Buttondown, Mailchimp, Kit, etc.). Until then the form shows "signup is not open yet" and sends nothing |
| `REPLACE_ME_CONTACT_EMAIL` | footer "contact" link | A public contact address, e.g. hello@checksumerror.io |

The six Instagram tiles are empty frames. Swap them for real post images once the account has posts, or delete that grid.

Prices ($34.99 tees, $62.99 hoodies) come from the launch-kit listings. If the pricing agent changes Etsy prices, update them here too.

## Going live on GitHub Pages
1. Put these files in the root of the `checksumerror.io` repo (or create it: github.com/new, name `checksumerror.io`). Commit and push to `main`.
2. Repo **Settings > Pages**: Source "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
3. Same page, **Custom domain**: `checksumerror.io` (the CNAME file already says this). Save.
4. At your domain registrar's DNS settings, add:
   - Four `A` records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Four `AAAA` records for `@` (optional, IPv6): `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
   - One `CNAME` record for `www` pointing to `pl8ypus.github.io`
   - Remove any other `A`/`AAAA`/`ALIAS` record on `@` (registrar parking pages).
5. Wait for DNS (minutes to a few hours), then tick **Enforce HTTPS** in Settings > Pages once it is clickable.
6. Recommended: verify the domain under your GitHub account (**Settings > Pages > Add a domain**) so no one else can claim it on Pages.
7. Check the link preview at https://www.opengraph.xyz/ after it is live.

Note: GitHub Pages on a **private** repo needs a paid GitHub plan (Pro). On the free plan, make the repo public.
