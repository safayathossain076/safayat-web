# Safayat's World: website files for www.safayatho.com

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The whole website (one page) |
| `favicon.svg` | Browser-tab icon |
| `logo-mark.svg` / `logo-mark.png` | Logo mark, also used as the phone home-screen icon |
| `photo.jpg` | Your portrait for the animated photo frame |

## Change your photo

Replace `photo.jpg` with another square portrait (at least 800 × 800 px, face centred).

## Add project details and photos

1. Put photos in the `projects` folder (JPG, about 1600 px wide), e.g. `projects/riedbahn-1.jpg`.
2. Open `index.html` and search for `const PROJECTS=[`.
3. Find the project and fill in its fields:
   - `summary`: a short description
   - `points`: key facts, e.g. `['142 km of LST cable','PT1 and PT2 planning']`
   - `photos`: the photo files, e.g. `['projects/riedbahn-1.jpg','projects/riedbahn-2.jpg']`
4. To show a funded startup, scholarship or research project, copy any entry and set
   `cat` to `'startup'`, `'scholarship'` or `'research'`. It appears in the Funded projects section automatically.

## Put it online (free, about 15 minutes)

**Option A: Netlify (easiest)**
1. Go to app.netlify.com/drop and drag this whole folder onto the page.
2. Create a free account to keep the site.
3. In Site settings › Domain management, add `safayatho.com` and `www.safayatho.com`.
4. At the company where you bought the domain, set the DNS records Netlify shows you. HTTPS is switched on automatically.

**Option B: GitHub Pages**
1. Create a public repository, upload these files.
2. Settings › Pages › deploy from the `main` branch.
3. Add `www.safayatho.com` as the custom domain and follow the DNS steps shown.

## Make the application form collect submissions

Without changes, the form prepares each registration as an email to `hello@safayatho.com`.
To receive submissions automatically instead:

1. Create a free form at formspree.io (or a similar service) and copy its endpoint URL.
2. Open `index.html`, search for `FORM_ENDPOINT = ''` and paste the URL between the quotes.
3. To use a different inbox, change `CONTACT_EMAIL` on the next line.

## Before launch

- Set up the `hello@safayatho.com` mailbox (or change it in `index.html`).
- Replace the footer links for Impressum and Privacy with real pages; German law requires both.
- Check the legal setup for receiving partner donations (gemeinnützige GmbH, Stiftung or e.V.).
