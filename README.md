# PDF First Website

Premium static website for PDF First by ASGENLABS. Ready for GitHub Pages.

## Files
- `index.html` — public developer/app website
- `privacy-policy.html` — public privacy policy
- `app-ads.txt` — AdMob authorized sellers file (replace placeholder publisher ID)
- `robots.txt` — allows normal crawling
- `assets/` — logo and screenshots

## IMPORTANT: AdMob app-ads.txt + GitHub Pages
AdMob crawls `app-ads.txt` from the ROOT of the developer website hostname.

For GitHub Pages, the safest setup is to publish this website from your user-site repository:

`YOUR_GITHUB_USERNAME.github.io`

Then your URLs become:
- Website: `https://YOUR_GITHUB_USERNAME.github.io/`
- Privacy Policy: `https://YOUR_GITHUB_USERNAME.github.io/privacy-policy.html`
- app-ads.txt: `https://YOUR_GITHUB_USERNAME.github.io/app-ads.txt`

A project site such as `https://YOUR_GITHUB_USERNAME.github.io/pdf-first/` places `app-ads.txt` under a subfolder, while AdMob normally checks the hostname root. Use the user-site repository or a custom domain for reliable app-ads.txt verification.

## AdMob setup
Open `app-ads.txt` and replace:

`pub-REPLACE_WITH_YOUR_ADMOB_PUBLISHER_ID`

with the personalized publisher ID/code snippet shown in your AdMob account.

Example format:
`google.com, pub-1234567890123456, DIRECT, f08c47fec0942fa0`

Do not copy the example ID.

## Deploy
1. Create a GitHub repository named exactly `YOUR_GITHUB_USERNAME.github.io`.
2. Upload the CONTENTS of this ZIP to the repository root.
3. Go to Settings → Pages.
4. Choose Deploy from a branch → `main` → `/ (root)`.
5. Save and wait for deployment.
6. Open `/app-ads.txt` in a browser and confirm it returns plain text.
7. Set this live site as the Developer Website in your Google Play listing.

## Before production
- Replace the AdMob publisher ID placeholder.
- Replace `support@asgenlabs.com` in HTML if your real support email is different.
- Update Google Play URL/button when the app is live.


## Privacy Policy
The website Privacy Policy buttons are linked to:
https://asgenlabs-ai.github.io/pdf-first-privacy/

## AdMob app-ads.txt
For AdMob verification, `app-ads.txt` must be available at the root of the developer website hostname listed in the app store.
If your developer website hostname is `asgenlabs-ai.github.io`, AdMob will look for:
`https://asgenlabs-ai.github.io/app-ads.txt`
A file only at `/pdf-first-privacy/app-ads.txt` or another project subpath may not satisfy the root-host requirement.
Replace the placeholder publisher ID in `app-ads.txt` with the exact line provided by AdMob before production.
