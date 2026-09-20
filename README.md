# Delirium in 30

A small GitHub Pages redirect for **www.deliriumin30.com**. The course is maintained at:

https://deliriumacademy.com/introduction-to-delirium/

This repository contains no copy of the clinical teaching, assessment or videos. Both the home page and unknown paths direct visitors to the Academy course. An immediate HTML redirect works without JavaScript; the visible link is a fallback. GitHub Pages serves a static HTML redirect, not a server-side HTTP 301. There are no analytics tags, cookies or external assets on this redirect page.

## Connect the domain at Porkbun

The intended GitHub Pages custom domain is `www.deliriumin30.com`.

- `CNAME` record: host `www`, value `amaclullich.github.io` (do not include the repository path).
- Four `A` records for the root domain, host `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
- Replace conflicting website records only; preserve unrelated email and verification records.
- Once DNS has propagated, check the domain in this repository’s Pages settings and enable **Enforce HTTPS** when the certificate is available.
- Check both `https://deliriumin30.com` and `https://www.deliriumin30.com` reach the course.

GitHub automatically redirects the root domain to the configured `www` domain when both DNS records are correct. Domain verification is also available in account Settings → Pages, using the TXT record supplied there.

Official guidance, checked 20 September 2026:
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https

## Maintenance

If the course’s canonical URL changes, update the refresh target, canonical link and fallback link in both HTML files. The course remains on Delirium Academy.
