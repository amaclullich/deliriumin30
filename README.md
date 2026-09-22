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

## Link previews and search

Every page carries Open Graph and X card tags, so a pasted deliriumin30.com link shows the Delirium in 30 card (the same image the course page uses). Every page also carries `noindex`, so the redirect pages do not compete with the course page in search results.

## Tagged channel links

Each folder below holds a copy of `index.html` whose redirect adds campaign tags (`utm_medium=referral`, `utm_campaign=launch`), so visits from each channel can be compared in Google Analytics under Traffic acquisition, Session source. Counts cover only visits where analytics are allowed to run, so use them to compare channels, not as absolute numbers.

| Link | utm_source |
| --- | --- |
| deliriumin30.com/lothian | lothian-induction |
| deliriumin30.com/shfa | shfa |
| deliriumin30.com/4at | the4at |
| deliriumin30.com/eda | eda |
| deliriumin30.com/students | edinburgh-programmes |
| deliriumin30.com/carehomes | care-homes |
| deliriumin30.com/fy | foundation-doctors |
| deliriumin30.com/li | linkedin |
| deliriumin30.com/x | x |
| deliriumin30.com/bsky | bluesky |
| deliriumin30.com/nes | nes-elfh |
| deliriumin30.com/standards | standards-bodies |
| deliriumin30.com/poster | qr-poster |

To add a channel, copy any channel folder, rename it, and change `utm_source` in the refresh line and the fallback link.

## Maintenance

If the course’s canonical URL changes, update the refresh target, canonical link, `og:url` and fallback link in `index.html`, `404.html` and every channel folder. The course remains on Delirium Academy.
