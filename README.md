# NOAM — Delhi Survival Guide · Deploy Guide

This folder is your complete website: 52 pages, ready to publish. You do **not**
need a terminal, Astro, or any coding tools. Vercel does everything for you.

## What's in here
- `public/` — all 52 web pages (this is the site). `index.html` is the home page.
- `package.json` and `vercel.json` — small config files that tell Vercel to build
  the search index automatically when it publishes. Leave them as they are.

## How to publish (about 10 minutes, all in the browser)

### 1. Put this folder on GitHub
The easiest no-terminal route:
1. Go to https://github.com and sign in (create a free account if needed).
2. Click the **+** (top right) → **New repository**. Name it `noam-delhi`,
   keep it Public or Private, click **Create repository**.
3. On the new repo page, click **uploading an existing file**.
4. Drag the **entire contents** of this deploy folder (the `public` folder,
   `package.json`, and `vercel.json`) into the upload area.
5. Click **Commit changes**.

### 2. Connect Vercel
1. Go to https://vercel.com and **Sign up with GitHub** (free Hobby plan is fine).
2. Click **Add New… → Project**.
3. Find your `noam-delhi` repo and click **Import**.
4. Vercel will read `vercel.json` automatically. You should see:
   - Build Command: `npm run build`
   - Output Directory: `public`
   Leave these as detected.
5. Click **Deploy**. Wait ~1 minute.

That's it. Vercel gives you a live URL like `noam-delhi.vercel.app`.
The search box will work on the live site (the index is built during deploy).

### 3. (Optional) Your own domain
In the Vercel project → **Settings → Domains**, add a domain you own
(e.g. `notonamap.com`) and follow the on-screen DNS steps.

## Updating the site later
Re-upload changed files to the same GitHub repo (same drag-and-drop).
Vercel re-deploys automatically within a minute.

## Notes
- Clean URLs are on: visitors see `/foreword`, not `/foreword.html`.
- The contact email in the footer is `notonamap@proton.me`.
- The Language page is currently the last page (its "Next" link is removed for now).
