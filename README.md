# HAMBRAM · The Nothing Religion

The website for HAMBRAM, the Nothing Religion.

Live: https://shivee999.github.io/thenothingreligion/

## What's here

| File | What it is |
|---|---|
| `index.html` | The whole site in one file: the book, the Daily Six, the blessings and the pledge |
| `og.png` | The picture people see when the link is shared on WhatsApp, X or Facebook |
| `.nojekyll` | Tells GitHub Pages to serve the files exactly as they are |

## Changing the site

Edit `index.html` and commit to `main`. GitHub Pages republishes in a minute or two.

## Connecting thenothingreligion.com

Do these steps in this order. If you add the DNS records before step 2, someone else can claim your domain on GitHub.

1. Verify the domain in your account: github.com/settings/pages → **Add a domain**. GitHub gives you a TXT record to add at your domain registrar.
2. In this repo: **Settings → Pages → Custom domain**, enter `thenothingreligion.com`, then **Save**.
3. At your domain registrar, add these DNS records:

   | Type | Name | Value |
   |---|---|---|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |
   | CNAME | www | shivee999.github.io |

4. When GitHub shows the DNS check has passed, tick **Enforce HTTPS**.
5. In `index.html`, change both `og.png` links from `https://shivee999.github.io/thenothingreligion/og.png` to `https://thenothingreligion.com/og.png`.

Never add a wildcard record such as `*.thenothingreligion.com`. GitHub warns that wildcard records let others take over your subdomains.

Source for the records: [GitHub Docs, Managing a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)
