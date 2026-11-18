# Sharesthesia site

Four static pages, no build step: `index.html`, `privacy.html`, `terms.html`,
`delete-account.html`, one `style.css`. Hosted on GitHub Pages for free.

## Put it online (once, ~10 minutes)

1. GitHub → **New repository** → name `sharesthesia-site`, **Public**, no
   README → Create.
2. Upload these files (Add file → Upload files → drag the five files → Commit).
3. Repository **Settings → Pages** → Source: **Deploy from a branch** →
   Branch `main`, folder `/ (root)` → Save. In a minute the site is at
   `https://<your-github-name>.github.io/sharesthesia-site/`.

## Your own domain (after buying sharesthesia.com)

4. **Settings → Pages → Custom domain**: type `sharesthesia.com` → Save.
   GitHub adds a `CNAME` file to the repo by itself.
5. At the registrar (Namecheap → Domain List → Manage → **Advanced DNS**),
   remove the parking records and add:
   - `A` record, host `@`, value `185.199.108.153`
   - `A` record, host `@`, value `185.199.109.153`
   - `A` record, host `@`, value `185.199.110.153`
   - `A` record, host `@`, value `185.199.111.153`
   - `CNAME` record, host `www`, value `<your-github-name>.github.io`
6. Back in Settings → Pages, wait for the DNS check to go green (minutes to
   an hour), then tick **Enforce HTTPS**.

The pages are then at `https://sharesthesia.com/privacy.html` and so on.
Those are the links for the app (ONB-3's Terms and Privacy), the Play
Console (Privacy policy URL, account-deletion URL) and the Google Cloud
consent screen (homepage + privacy URL). For the consent screen the domain
also has to be verified once in Google Search Console: add a property for
`sharesthesia.com`, choose the DNS TXT method, paste the TXT record at
Namecheap, Verify.

## Editing later

Change a file on GitHub, commit; the site updates within a minute. Change
the "Last updated" line at the top of a page when its words change.
