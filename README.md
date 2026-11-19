# GTA 6 Moments — website files

Static site for the GTA 6 Moments channel. Deploy it free on GitHub Pages so
TikTok can verify the domain for the developer app "GTA 6 Moments"
(app ID 7709837288129398804).

## Files

- `index.html` — channel landing page (links to TikTok @spyd3rgaming1 and YouTube Gta Moments)
- `terms.html` — Terms of Service
- `privacy.html` — Privacy Policy
- `logo.png` — channel logo (800x800)

## Deploy (GitHub Pages) — IMPORTANT: use a USER site, not a project site

TikTok's URL verification needs its verification file at the **root** of the
domain. On GitHub Pages that only works with a **user site**: a repository
named exactly `<your-github-username>.github.io`. A project site
(`<username>.github.io/<repo>/`) puts files under a sub-path, and TikTok's
root check will fail.

Steps:

1. Create a free GitHub account if you don't have one: https://github.com/signup
2. Create a new public repository named exactly `<your-github-username>.github.io`
   (replace `<your-github-username>` with your GitHub username).
3. Upload all files from this folder into that repository (web upload is fine:
   repository page → Add file → Upload files).
4. Go to repository Settings → Pages → Source: Deploy from a branch,
   Branch: main, Folder: / (root). Save.
5. Wait a minute, then open `https://<your-github-username>.github.io/` —
   the site should be live.

## URLs to put in the TikTok developer app form

Once the site is live at `https://<your-github-username>.github.io/`:

- Web/Desktop URL: `https://<your-github-username>.github.io/`
- Terms of Service URL: `https://<your-github-username>.github.io/terms.html`
- Privacy Policy URL: `https://<your-github-username>.github.io/privacy.html`

## TikTok URL verification file

After entering the Web/Desktop URL in the TikTok developer portal, TikTok
gives you a verification file to host (or a DNS record). For the file method:

1. Download the verification file TikTok provides (it looks like
   `tiktok-developers-site-verification=XXXX.txt` or similar).
2. Upload it to the **root** of this same repository (next to index.html).
3. Wait for GitHub Pages to publish it, then open
   `https://<your-github-username>.github.io/<that-filename>` in a browser
   to confirm it loads.
4. Click Verify in the TikTok portal.

Do NOT rename the verification file — TikTok checks the exact name.

## Demo video (still blocked)

The TikTok app review also asks for a demo video showing the end-to-end
Login Kit + Content Posting API flow. That can only be recorded once the
posting integration is built and working, which happens after the app is
approved. It is a later step, not part of this site.
