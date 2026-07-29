# intotheechoside.com — official site (GitHub Pages)

Single-file landing page announcing the re-release, the mobile app launch, and
the upcoming Echoside Judge referee app.

## Deploy to GitHub Pages

1. Create a repo (e.g. `intotheechoside-site`), push these files:

       git init && git add -A && git commit -m "Into the Echoside site"
       git branch -M main
       git remote add origin https://github.com/kirkcreason-dev/intotheechoside-site.git
       git push -u origin main

2. Repo → Settings → Pages → Source: "Deploy from a branch" → `main` / root.
3. Custom domain: the included `CNAME` file already says `www.intotheechoside.com`.
   In Settings → Pages, enter `www.intotheechoside.com` and check "Enforce HTTPS"
   (available after DNS propagates).

## DNS records (at your domain registrar)

| Type  | Host | Value                     |
|-------|------|---------------------------|
| CNAME | www  | kirkcreason-dev.github.io        |
| A     | @    | 185.199.108.153           |
| A     | @    | 185.199.109.153           |
| A     | @    | 185.199.110.153           |
| A     | @    | 185.199.111.153           |

The A records make the bare domain `intotheechoside.com` redirect to `www`.

## Assets (delivered and in place)

- `hero.jpg` — box/key art for the framed slot in the Re-Release section (Tom Wood art; ~1440px wide)
- `app-screenshot.png` — phone screenshot of the app (portrait)
- `og-image.jpg` — social share image, 1200×630
- `favicon.png` — 64×64 logo mark
- Official App Store / Google Play badge images once the store listings exist
  (Apple and Google require their official badge artwork at launch; the current
  placeholder badges are styled stand-ins marked "coming soon")
- Any card art / character renders for extra sections, if you want them

Every asset slot degrades gracefully — missing images simply don't render, and
labeled placeholder boxes show where they'll go.

## Mailing list

The Notify Me form is front-end only. To make it live, point the form `action`
at a Mailchimp/Buttondown/ConvertKit endpoint (each provides a copy-paste form
URL), or tell me which service you use and I'll wire it.
