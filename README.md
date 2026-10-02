# JP+ Pharmaceutical Journal Website

A responsive, static multi-page journal website built with HTML, CSS, and vanilla JavaScript. Designed for free hosting on GitHub Pages or Netlify.

## Included pages
- Home
- About the journal
- Current issue
- Archives
- Manuscript submission
- Editorial policies
- Contact

## Before publishing
1. Confirm the journal's actual name, aims, scope, publisher identity, editorial board, and contact email.
2. Review and approve every editorial policy. The policy page is a starter framework, not legal or ethics advice.
3. In `contact.html`, replace `journal.email@example.com` with the journal's dedicated email.
4. In `submit.html`, create a Google Form and replace the placeholder with its embed URL. See instructions below.
5. Remove any claims (such as no APC, peer-review status, indexing, ISSN, DOI, or publication frequency) that are not yet verified and operational.
6. Add real article metadata and PDF links only after publication approval.

## Configure Google Forms
1. Create a Google Form with author, manuscript, abstract, declarations, and secure manuscript-file/link fields.
2. In Google Forms, choose **Send** → **Embed HTML**.
3. Copy the URL from the iframe's `src` attribute.
4. Open `submit.html`. Find the `YOUR_GOOGLE_FORM_EMBED_URL` placeholder in the commented iframe block.
5. Uncomment the iframe and replace the placeholder with your form URL.
6. Set an appropriate iframe height. Test the form on desktop and mobile.
7. Restrict response spreadsheet access to authorized editorial staff. Do not request unnecessary sensitive personal information. For manuscript files, use a controlled-access storage workflow rather than a public folder.

## Deploy to GitHub Pages
1. Create a GitHub repository (for example, `pharma-journal`).
2. Upload the contents of this folder to the repository root (so `index.html` is at the root).
3. In repository **Settings → Pages**, select **Deploy from a branch**, choose `main` and `/ (root)`, then save.
4. Wait for the deployment URL shown in Pages settings.
5. Test all navigation links, the submission form, contact email, and mobile layout.

## Deploy to Netlify
Drag the project folder into Netlify's manual deploy area, or connect the Git repository. No build command is required; publish directory is the project root.

## Customization
- Edit text in the HTML files.
- Change colors and layout in `assets/styles.css` (CSS variables are at the top).
- The site uses Google Fonts when online and falls back to system fonts if unavailable.
- No backend, database, or server-side code is included.
