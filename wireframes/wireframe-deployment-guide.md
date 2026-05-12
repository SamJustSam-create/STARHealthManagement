# Wireframe Deployment Guide
**STAR Health — Homepage, RTT Page & Shop Wireframes**
**Prepared by:** Byte Development
**Original Date:** February 2026
**Last Updated:** May 2026 (added Homepage wireframe; switched recommended option to GitHub Pages to match active deployment; pre-flight checklist expanded)
**Files:**
- `wireframes/homepage-wireframe.html` — Homepage
- `wireframes/rtt-page-wireframe.html` — RTT Landing Page
- `wireframes/shop-wireframe.html` — E-Commerce Shop Page

---

## Overview

This document outlines the options for sharing all three wireframes with the client (Thomas, STAR Health) for review and feedback. Each wireframe is a self-contained HTML file. No server, build process, or framework is required — they run directly in a browser.

The three wireframes are deployed **together as a single site** (Options 2–4), each accessible at its own path. This keeps everything under one URL structure, makes cross-referencing easier for Thomas, and means only one deployment to manage when iterating.

**Active deployment:** This project is deployed via **GitHub Pages** (Option 3). The live wireframe URLs sent to Thomas are:
- `https://samjustsam-create.github.io/STARHealthManagement/wireframes/homepage-wireframe.html`
- `https://samjustsam-create.github.io/STARHealthManagement/wireframes/rtt-page-wireframe.html`
- `https://samjustsam-create.github.io/STARHealthManagement/wireframes/shop-wireframe.html`

**One dependency to note:** All three files load Barlow Condensed and Inter from Google Fonts via a `<link>` tag. The viewer must have an active internet connection for the typography to render correctly. Offline viewing will fall back to system fonts and will not represent the intended design accurately.

---

## Deployment Options

Four approaches are covered, ordered from simplest to most controlled. The recommended option for this project — and the one currently in use — is [Option 3 — GitHub Pages](#option-3--github-pages-recommended).

---

### Option 1 — Direct File Share (Email / Cloud Link)

**Best for:** Quick, informal sharing. No setup required.

**How to do it:**

1. Attach `homepage-wireframe.html`, `rtt-page-wireframe.html`, and `shop-wireframe.html` to a single email to Thomas, **or**
2. Upload all three files to a shared Google Drive / Dropbox / iCloud folder and send Thomas the folder link.

**Thomas's steps to view each:**
1. Download the file he wants to review.
2. Open it in a browser (double-click, or right-click → Open With → Browser).
3. Ensure he is connected to the internet so fonts load.

**Pros:**
- Zero setup time for you.
- No third-party account required.

**Cons:**
- Requires Thomas to download and open a local file — a friction point.
- No live URL to reference or link back to.
- If you update the wireframe, you must re-send the file.

---

### Option 2 — Netlify Drop

**Best for:** Sharing live URLs with zero configuration when version control isn't needed.

Netlify Drop lets you deploy an entire folder instantly by dragging it into the browser. All three wireframes are deployed together as a single site and become accessible at their own paths — one deployment, three URLs to send Thomas.

**Steps (no account):**

1. Go to **[netlify.com/drop](https://app.netlify.com/drop)** in your browser.
2. Drag and drop the entire **`wireframes/` folder** (not individual files) into the drop zone.
3. Netlify generates a live site URL immediately (e.g., `https://random-name-123.netlify.app`).
4. All three wireframes are now accessible at:
   ```
   https://random-name-123.netlify.app/homepage-wireframe.html
   https://random-name-123.netlify.app/rtt-page-wireframe.html
   https://random-name-123.netlify.app/shop-wireframe.html
   ```
5. Send Thomas all three URLs.

> **Note:** Without an account, the site URL expires after 24 hours. Use the steps below for a persistent link.

**Steps with a free Netlify account (persistent URLs):**

1. Sign up for a free Netlify account at [netlify.com](https://netlify.com).
2. From the dashboard, go to **Sites → Add new site → Deploy manually**.
3. Drag the entire `wireframes/` folder into the deploy zone.
4. Rename the site to something readable: **Site settings → General → Site details → Change site name** (e.g., `star-health-wireframes`).
5. All three wireframes are now live at permanent URLs:
   ```
   https://star-health-wireframes.netlify.app/homepage-wireframe.html
   https://star-health-wireframes.netlify.app/rtt-page-wireframe.html
   https://star-health-wireframes.netlify.app/shop-wireframe.html
   ```

**To redeploy after changes to any wireframe:**
- Go to your site in the Netlify dashboard → **Deploys** tab.
- Drag the updated `wireframes/` folder into the drop zone — all URLs stay the same.

**Pros:**
- All wireframes live under one deployment — one place to manage, update, and share.
- Instant live URLs — no download required for Thomas.
- Works on desktop and mobile.
- Free tier is sufficient for wireframe review.

**Cons:**
- Requires a Netlify account for a stable URL (random URLs expire after 24 hours).
- Site is publicly accessible — no password protection on the free tier.

---

### Option 3 — GitHub Pages (Recommended — Currently In Use)

**Best for:** Keeping all wireframes version-controlled alongside the project, with stable URLs at no cost.

This is the option currently in use for this project. Because all three files already live in the `wireframes/` folder, pushing that folder to a GitHub repository automatically gives each wireframe its own path — no extra configuration needed.

**Steps:**

1. Create a GitHub repository for the STAR Health project (or use an existing one).
2. Push the entire `wireframes/` folder to the repo:
   ```bash
   git add wireframes/
   git commit -m "Add homepage, RTT, and shop wireframes"
   git push
   ```
3. In the repo on GitHub: **Settings → Pages → Source → Deploy from a branch**.
4. Select the `main` branch and `/root` as the source folder.
5. GitHub publishes the site and all three wireframes are accessible at their own paths:
   ```
   https://your-username.github.io/repo-name/wireframes/homepage-wireframe.html
   https://your-username.github.io/repo-name/wireframes/rtt-page-wireframe.html
   https://your-username.github.io/repo-name/wireframes/shop-wireframe.html
   ```
6. Share all three URLs with Thomas.

**To update any wireframe:**
- Push a new commit with the updated HTML file(s).
- GitHub automatically redeploys within ~60 seconds. URLs do not change.

**Pros:**
- All three wireframes versioned together — full history of every iteration of every page.
- Stable URLs that persist as long as the repo is public.
- Free with a public repository.

**Cons:**
- More setup than Netlify Drop.
- Repository must be public for GitHub Pages to work on the free plan (private repos require GitHub Pro).
- URL includes your GitHub username and repo name — slightly less professional for client sharing.

---

### Option 4 — Railway

**Best for:** When you want a persistent, production-like deployment that mirrors the environment Railway will likely host the final STAR Health site on — useful if you intend to use Railway for the live project and want to validate the workflow early.

Railway is a cloud application platform built for server-side apps. Because it expects a runnable process rather than a static file drop, deploying a plain HTML file requires a minimal Node.js shim to serve it. The setup takes around 10–15 minutes but results in a stable HTTPS URL, Git-backed deploys, and a platform you'll already know by the time the real site needs deploying.

---

#### What You'll Need

- A [Railway account](https://railway.app) (free Hobby plan — includes $5/month credit, sufficient for wireframe review)
- A GitHub account
- Node.js installed locally (to initialise the project)
- The [Railway CLI](https://docs.railway.app/guides/cli) (optional, but covered below)

---

#### Step 1 — Prepare the Project Files

Railway needs a runnable Node.js project. The simplest approach is the [`serve`](https://www.npmjs.com/package/serve) package, which acts as a lightweight static file server.

Inside the `wireframes/` folder, create two new files alongside the HTML files:

**`package.json`**
```json
{
  "name": "star-health-wireframes",
  "version": "1.0.0",
  "scripts": {
    "start": "serve . --listen $PORT"
  },
  "dependencies": {
    "serve": "^14.2.4"
  }
}
```

**`railway.json`** *(optional but recommended — pins the build config)*
```json
{
  "$schema": "https://railway.app/railway.schema.json",
  "build": {
    "builder": "NIXPACKS"
  },
  "deploy": {
    "startCommand": "npm start",
    "restartPolicyType": "ON_FAILURE"
  }
}
```

Your `wireframes/` folder should now look like this:

```
wireframes/
├── homepage-wireframe.html
├── rtt-page-wireframe.html
├── shop-wireframe.html
├── package.json
└── railway.json
```

> **How it works:** Railway's Nixpacks builder detects `package.json`, runs `npm install` to pull in `serve`, then executes `npm start`. The `serve` package hosts the entire folder as a static site on the port Railway assigns via the `$PORT` environment variable — all three HTML files are served automatically.

---

#### Step 2 — Push to GitHub

Railway deploys from a GitHub repository. If the project isn't in one yet:

```bash
# From the STAR Health Management project root
git init
git add .
git commit -m "Initial commit — homepage, RTT, and shop wireframes"
```

Create a new repository on [github.com](https://github.com/new) (private is fine — Railway supports private repos), then push:

```bash
git remote add origin https://github.com/your-username/star-health-wireframe.git
git branch -M main
git push -u origin main
```

---

#### Step 3 — Create a Railway Project and Deploy

**Via the Railway dashboard (no CLI required):**

1. Log in at [railway.app](https://railway.app) and click **New Project**.
2. Select **Deploy from GitHub repo**.
3. Authorise Railway to access your GitHub account if prompted.
4. Select the `star-health-wireframe` repository.
5. Railway detects `package.json`, builds automatically using Nixpacks, and deploys.
6. Once the build completes, go to **Settings → Networking → Generate Domain**.
7. Railway generates a public URL (e.g., `https://star-health-wireframe.up.railway.app`).

**Via the Railway CLI (faster for future redeployments):**

```bash
# Install the CLI (once only)
npm install -g @railway/cli

# Log in
railway login

# Link the local folder to your Railway project
railway link

# Deploy
railway up
```

The CLI prints the deployment URL on completion.

---

#### Step 4 — Access All Wireframes

The deployed URL serves the `wireframes/` folder root. All three files are accessible at their own paths — send Thomas all three links:

```
https://star-health-wireframes.up.railway.app/homepage-wireframe.html
https://star-health-wireframes.up.railway.app/rtt-page-wireframe.html
https://star-health-wireframes.up.railway.app/shop-wireframe.html
```

> There is no `index.html`, so the root URL (`https://star-health-wireframes.up.railway.app`) will return a directory listing. This is fine for internal use — just send Thomas the three direct file links above.

---

#### Step 5 — Redeploying After Changes

Railway redeploys automatically on every push to the connected branch:

```bash
# After editing either wireframe
git add wireframes/
git commit -m "Update wireframes — incorporate Thomas feedback"
git push
```

Railway detects the push, rebuilds, and updates the live URL within ~30 seconds. The URL does not change.

---

#### Pros
- Persistent HTTPS URL with zero manual redeployment after the initial setup.
- Git-backed — every deploy is tied to a commit, giving you a clear history of wireframe iterations.
- Mirrors the likely production environment if Railway is used for the final site.
- Private GitHub repos are fully supported.

#### Cons
- More upfront setup than Netlify Drop (~10–15 min vs. ~2 min).
- Requires a `package.json` shim — slightly over-engineered for a single HTML file at wireframe stage.
- Railway's Hobby plan is free but requires a credit card on file; usage above the $5/month free allowance is billed (extremely unlikely for a static wireframe with low traffic).
- No built-in password protection — the URL is publicly accessible once a domain is generated.

---

## Recommendation Summary

| Option | Setup Time | Requires Account | Live URL | Git-backed | Best For |
|---|---|---|---|---|---|
| 1 — Email / File Share | None | No | No | No | Quick internal check |
| 2 — Netlify Drop | < 2 min | Optional | Yes | No | Throwaway preview links |
| **3 — GitHub Pages** | **~10 min** | **Yes (GitHub)** | **Yes** | **Yes** | **Client review (currently in use)** |
| 4 — Railway | ~15 min | Yes (Railway + GitHub) | Yes | Yes | Production-aligned, private repo |

**Current state:** Option 3 (GitHub Pages) is the active deployment for this project. The repository is already configured and `.nojekyll` is in place, so any push to `main` is reflected at the live URLs within ~60 seconds. No further setup needed for ongoing iteration.

**If Railway becomes the intended production platform:** Migrate to Option 4 closer to the final site build to validate the deploy workflow there. The extra setup time is worthwhile if it means the production deployment process is already understood and tested before go-live.

---

## Preparing the Files for Client Delivery

Before sharing, run a pre-flight check on all three wireframes:

**Homepage (`homepage-wireframe.html`)**
- [ ] Opens correctly in Chrome and Firefox.
- [ ] Hero, course cards, About strip, and footer sections reflow cleanly at narrow widths.
- [ ] Primary navigation links resolve to the correct pages (RTT, Shop, Fire Safety once added).
- [ ] "About SHM" / "Learn More About Us" buttons — pending Thomas's decision on whether to build an About page or remove these. Do not ship to client without resolving.
- [ ] Yellow wireframe annotation bar is visible at the top.

**RTT Page (`rtt-page-wireframe.html`)**
- [ ] Opens correctly in Chrome and Firefox.
- [ ] Accordion opens and closes on click; all panels start collapsed.
- [ ] Hero, UVP grid, audience, and form sections reflow cleanly at narrow widths.
- [ ] Yellow wireframe annotation bar is visible at the top.
- [ ] UVP grid — Thomas's amendments and additions from 2026-03-31 incorporated (pending confirmed list).

**Shop Page (`shop-wireframe.html`)**
- [ ] Opens correctly in Chrome and Firefox.
- [ ] Category filter pills correctly show and hide product cards on click.
- [ ] Product count label updates to match filtered results.
- [ ] Cart icon is visible in the nav.
- [ ] Hero, product grid, and featured kit section reflow cleanly at narrow widths.
- [ ] Yellow wireframe annotation bar is visible at the top.

**All three files**
- [ ] "For Review Only — Not Final Design" label is present in each.
- [ ] Fonts render correctly (confirms internet connection is active).
- [ ] All image placeholders reference dimensions consistent with `Image-Assets-Spec.md`.

---

## Presenting the Wireframes to Thomas

### Suggested Message (Email / WhatsApp)

> Hi Thomas,
>
> I've put together initial wireframes for the homepage, the RTT page, and the shop — links below:
>
> **Homepage:** [homepage-wireframe link]
> **RTT Landing Page:** [rtt-page-wireframe link]
> **Shop Page:** [shop-wireframe link]
>
> These are mid-fidelity layouts showing the full page structure, colour direction, and typography. Photography placeholders show where your imagery will sit once the first batch comes through.
>
> A few interactive elements to try:
> - Homepage: Click through the course cards to see how each links into the deeper pages.
> - RTT page: Click the rows in the "What the Training Covers" section to expand each module.
> - Shop page: Use the category filter buttons (Trauma Kits, Haemorrhage Control, etc.) to see how the product grid filters down.
>
> A few things I'd love your feedback on:
> 1. Does the homepage tone strike the right balance between the RTT credibility and the general-public approachability?
> 2. Does the RTT page tone and layout feel right for your audience?
> 3. Are the training module names accurate, or do any need changing?
> 4. On the shop — does the product category breakdown make sense? Anything missing or out of place?
> 5. Are the product names and descriptions representative of what's in the Shopify store?
>
> Happy to jump on a quick call to walk through all three together.
>
> Samuel

### Feedback to Collect

Steer Thomas toward structured feedback on these specific points:

**Homepage**

| Area | Question for Thomas |
|---|---|
| Tonal balance | Does the page strike the right balance between RTT credibility and general-public approachability? |
| Course visibility | Are the upcoming courses / courses offered surfaced clearly enough on the page? |
| About SHM buttons | Should these resolve to a dedicated About page, or be removed entirely? |
| Hero direction | Does the hero imagery direction land the SHM brand without leaning too far into either RTT or general first aid? |
| Nav ordering | Is RTT in the right position in the nav? (Prior feedback suggested promoting it.) |

**RTT Page**

| Area | Question for Thomas |
|---|---|
| Overall tone | Does it feel professional and credible without being too aggressive? |
| Section order | Is the page flow logical for how his audience thinks about RTT? |
| Audience list | Are all target roles listed? Any to remove? |
| Training modules | Are the five module names correct? Any additions or changes? |
| CTA copy | Is "Enquire About RTT Training" the right call-to-action label? |
| Form fields | Are the five enquiry fields sufficient, or is something missing? |

**Shop Page**

| Area | Question for Thomas |
|---|---|
| Category names | Do the six filter categories match how products are organised in Shopify? |
| Featured product | Is the "RTT Trauma Response Kit" the right product to spotlight in the hero and featured section? |
| Product cards | Are the placeholder names and descriptions representative of the real catalogue? |
| Trust signals | Are the four trust strip items (Secure Checkout, Shipping, RTO-Verified, 48hr Dispatch) accurate? |
| "Powered by Shopify" | Is Thomas comfortable showing this in the footer, or should it be omitted? |

---

## After Thomas's Feedback

1. Note all feedback from Thomas, separating homepage changes, RTT page changes, and shop page changes.
2. Update whichever wireframe(s) need revisions — `homepage-wireframe.html`, `rtt-page-wireframe.html`, `shop-wireframe.html`, or any combination.
3. Redeploy:
   - **GitHub Pages (current):** Push the updated files — URLs update automatically within ~60 seconds.
   - **Netlify:** Drag the updated `wireframes/` folder into the Deploys drop zone — all URLs stay the same.
   - **Railway:** Push the updated files — URLs update automatically within ~30 seconds.
4. Notify Thomas that the wireframes have been updated and ask for sign-off on all three before proceeding to high-fidelity Figma mockups.

---

*This guide covers wireframe-stage sharing only. Production deployment planning will follow once the website platform is confirmed with Dom.*
