# Kids Screen‑Time Tracker — HTTPS Hosting Guide

This folder is ready to deploy over **HTTPS** so the app can install as a PWA and use the service worker.

## Option A — Netlify Drop (fastest, no account needed)
1. Go to **https://app.netlify.com/drop** (HTTPS).
2. Drag the **entire folder** into the page (the folder that contains `index.html`, `manifest.webmanifest`, `sw.js`, and `icons/`).
3. Netlify gives you a **public HTTPS URL** immediately.
4. Open that URL on your phone/computer → tap **Install app**.

## Option B — GitHub Pages (free, permanent)
1. Create a new repo on GitHub (Public is fine).
2. Upload all files from this folder to the repo **root**.
3. In **Settings → Pages**, set Source to **Deploy from a branch**, Branch **main** (or `gh-pages`), and Folder **/** (root). Save.
4. Wait 1–2 minutes; your site will be live at `https://<your-username>.github.io/<repo-name>/` (HTTPS).
5. Visit the URL → the **Install app** button appears when eligible.

## Option C — Replit (quick HTTPS dev link)
1. Go to **https://replit.com** → Create Repl → **HTML, CSS, JS**.
2. Upload the files (`index.html`, `manifest.webmanifest`, `sw.js`, and `icons/` folder).
3. Click **Run** → Replit shows an **HTTPS** preview URL.

## Local HTTPS (advanced)
Service workers require a **secure context**. `file://` won’t work. If you must host locally over HTTPS, use a dev server with SSL (for example, Node + mkcert). Most users will find Netlify Drop or GitHub Pages much easier.

---

## Using the App
- Set each kid’s weekday/weekend limits, pick **Day**, press **Start**.
- Use **Rewards** to add **points**; click **Claim from Jar** on a day to convert points into bonus minutes.
- **Settings** → pick alarm (fart/boop/bell/kazoo), adjust volume/mute, optional **PIN**.
- Data saves to your browser (**localStorage**) on the device.

If you want me to pre-host this for you on GitHub Pages/Netlify, just share a preferred site name and I’ll prep the exact steps you can click through.