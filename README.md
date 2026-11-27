# checksumerror.io

Checksum Error’s coming-soon page. Static HTML and CSS with local fonts and images. Serve this directory as the web root.

## Coming-soon launch

- [ ] Confirm the brand’s Instagram account. In `index.html`, replace the homepage link marked `REPLACE_ME_INSTAGRAM` with the verified profile URL and remove the pending note. The planned handle is `@checksumerror`.
- [ ] Review the five previews. The Ship It preview omits the tool name flagged for review in the listing draft. The approved print wording goes at `REPLACE_ME_SHIP_IT_ART`. Confirm the public privacy and operator details with your adviser using the actual hosting setup.
- [ ] In Cloudflare **Workers & Pages**, create or select the Pages project for [Pl8ypus/checksumerror.io](https://github.com/Pl8ypus/checksumerror.io). Set production branch to `main`, framework preset to **None**, leave the build command and root directory blank, and set the output directory to `.`. This repo has `index.html` at its root. Review the files and then commit and push to the production branch. [Cloudflare Git integration guide](https://developers.cloudflare.com/pages/get-started/git-integration/)
- [ ] In **Pages > Custom domains**, add `checksumerror.io`. If the apex domain is new to Cloudflare DNS, add the zone and use its assigned nameservers at the registrar. Let Pages create the DNS record and wait for the domain and certificate to become active. [Cloudflare custom domains guide](https://developers.cloudflare.com/pages/configuration/custom-domains/)
- [ ] Check the production deployment and `https://checksumerror.io/` on a phone. Verify the Instagram link, social card, HTTP 404 for a missing path, `robots.txt`, and `sitemap.xml`. Check for unexpected cookies or requests, including any injected by hosting settings.

## After the preview

- [ ] `REPLACE_ME_ETSY_LINKS` marks where to add purchase links after the shop and listings are live. Prices belong on Etsy.
- [ ] `REPLACE_ME_EMAIL_SIGNUP` marks the disabled preview. Before collecting addresses, confirm the controller and processor details, publish and link the reviewed privacy policy, add signup consent wording, and configure the provider’s double opt-in and unsubscribe. Test a signup and an unsubscribe using a controlled email address.
