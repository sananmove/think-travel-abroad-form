# Think Travel Abroad: Lead Form

A single-page request-for-information form. Submissions are saved to a Google Sheet through Google Apps Script.

## Publish on GitHub Pages

1. Sign in to github.com and click **New** (or go to github.com/new).
2. Name the repository, for example `think-travel-abroad-form`.
3. Choose **Public** (GitHub Pages is free for public repositories) and click **Create repository**.
4. Click **uploading an existing file**, drag in `index.html` and `README.md`, then click **Commit changes**.
5. Open **Settings > Pages**.
6. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then click **Save**.
7. Wait 1 to 2 minutes and refresh the page. The live address appears at the top:
   `https://YOUR-USERNAME.github.io/think-travel-abroad-form/`

## Before you go live

- Open `index.html` and paste your Apps Script Web App URL into `CONFIG.endpoint`. Until you do, the form shows a "not connected yet" message and will not send submissions.
- Make sure the Apps Script deployment is set to **Who has access: Anyone**.
- Test one submission and check the Leads tab in your Google Sheet.

## Notes

- Anyone with the link can view the page. The Apps Script URL is visible in the page source, so anyone can send entries to your sheet. The honeypot field filters out most bots, but consider adding a CAPTCHA later if spam appears.
- To update the site, edit `index.html` on GitHub (pencil icon) and commit. The live page updates within a few minutes.
- For your own domain (for example, `apply.thinktravelabroad.com`), use **Settings > Pages > Custom domain** after the site is live.
