# Pre-iscrizioni / Intresseanmälan — form

Bilingual (Italian / Swedish) **interest / pre-registration** form for **Italienska Skolan
Stockholm**. Ported from a Cognito Forms form
(<https://www.cognitoforms.com/ItalienskaSkolanStockholm/PreIscrizioni>) to the same self-hosted
stack as the Scuola del Sabato form: a static HTML frontend + Google Apps Script backend.

| File | Purpose |
|------|---------|
| `pre-iscrizioni.html` | The bilingual pre-registration form (self-contained HTML + CSS + JS) |
| `grazie.html` | Bilingual thank-you page (language via `?lang=it\|sv`) |
| `logo-italienska-skolan.png` | School logo (banner + inline in emails) |

No payment, no course eligibility, no test — this is a manifestazione d'interesse.
No build step: open the HTML directly or serve statically. Served via GitHub Pages at
<https://italienska-skolan.github.io/pre-iscrizioni-form/pre-iscrizioni.html>.

The Google Apps Script backend (`Code.gs`) is kept **out of this public repo** (see `.gitignore`).

## Local dev
```bash
python3 -m http.server 3004
```
Then open `http://localhost:3004/pre-iscrizioni.html`.
