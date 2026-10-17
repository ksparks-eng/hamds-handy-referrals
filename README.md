# Hamd's Handy Referrals – static site

Plain HTML + CSS, no build step. Intended URL: https://hamdtransportation.com/referrals/

## Files
- index.html – home (hero, services, how it works, request form)
- hvac.html, plumbing.html, locksmith.html, towing.html, mobile-mechanic.html, roadside.html – service pages
- providers.html – "Join our provider network"
- styles.css, assets/crest.png, assets/favicon.png
- previews/ – screenshots only; no need to upload

## Forms (FormSubmit)
Both forms post to https://formsubmit.co/ksparks@hamdtransportation.com (no account needed).
- Subjects: "New customer request - Hamd's Handy Referrals" (index + 6 service pages), "New provider signup - Hamd's Handy Referrals" (providers.html)
- _next redirects to https://referrals.hamdtransportation.com/thanks.html; _template=table; reCAPTCHA left ON (FormSubmit recommends it).
- ACTIVATION: the first submission makes FormSubmit email ksparks@hamdtransportation.com a confirmation link. Click it once; until then nothing is delivered.

## Upload
1. Unzip hhr_site.zip.
2. The zip already contains a `referrals/` folder. Upload that folder into the hamdtransportation.com web root
   (cPanel File Manager / FTP: usually `public_html/`, giving `public_html/referrals/`).
3. (If uploading from `site/` instead, skip `previews/`.)
4. Visit https://hamdtransportation.com/referrals/ and test the phone link and both forms.

Website builders (Wix, Squarespace, GoDaddy Builder) can't host a raw folder like this: either
paste each page's content into new builder pages, or point a subdomain (e.g. referrals.hamdtransportation.com)
at a free static host like Netlify or Cloudflare Pages and drop the folder in.

All links are relative, so the folder works at any path.
