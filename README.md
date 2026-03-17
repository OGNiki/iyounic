# iYOUnic — Traction Landing Page

A premium, single-page traction site for iYOUnic: a beauty-tech platform that transforms makeup inspiration into personalized, guided experiences.

## 🚀 Live Site

[https://ogniki.github.io/iyounic/](https://ogniki.github.io/iyounic/)

---

## Setup

### 1. Tally Waitlist Form

1. Go to [tally.so](https://tally.so) and create a new form with:
   - First Name *(required)*
   - Last Name *(required)*
   - Email *(required)*
   - Makeup skill level *(multiple choice)*: Beginner / Intermediate / Beauty enthusiast
   - What best describes your makeup struggles? *(free text, optional)*

2. Connect to Airtable via Tally's Integrations tab

3. Get your form ID from the URL: `tally.so/r/**XXXXXXXX**`

4. In `index.html`, replace `XXXXXXXX` in the iframe `data-tally-src` with your form ID

5. Uncomment the Tally script in `<head>`:
   ```html
   <script async src="https://tally.so/widgets/embed.js"></script>
   ```

### 2. Contact Email

Update `hello@iyounic.com` in the footer with your real contact email.

### 3. GitHub Pages

Enable GitHub Pages in repo Settings → Pages → Source: `main` branch, `/ (root)`.

---

## Tech Stack

- Plain HTML/CSS/JS — no build tools, no dependencies
- Google Fonts (Cormorant Garamond + Inter) via CDN
- Tally.so for waitlist form (with Airtable integration)
- GitHub Pages for hosting

## Customization

| What | Where |
|------|-------|
| Colors | CSS `:root` variables at top of `<style>` |
| Logo/wordmark | Search for `.wordmark` — swap for `<img>` when logo is ready |
| Copy | All inline in HTML — clearly sectioned with comments |
| Form fields | Update in Tally, then swap the form ID |

---

*Built for traction. Ready to evolve.*
