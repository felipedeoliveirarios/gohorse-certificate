# Go Horse Certificate

A free certification exam based on the principles of eXtreme Go Horse (XGH).

## Run

Open `index.html` in your browser. No installation, build, backend, or database is required.

The HTML includes all application code, translations, the logo, and the certificate QR code. The Ko-fi widget loads from Ko-fi's CDN, with a plain support link as a fallback.

## Features

- Portuguese, Spanish, English, French, and Italian, including questions and certificates.
- Browser language detection, with English as the fallback.
- Light/dark switch and saved language/theme preferences.
- Ten questions; five correct answers are enough to pass.
- A personalized A4 landscape certificate (297 × 210 mm) with the logo at the top left, printable or savable as a one-page PDF.
- A certificate “validation” QR code that leads to a rickroll.
- Ko-fi support button: https://ko-fi.com/E1E2ZQY6A

Changing language preserves the current question, selected answer, score, and entered name. Refreshing the page starts a new exam; only language and theme preferences persist.

## Host

Serve `index.html` from any static web host. The site does not require server-side routing or environment variables.

### GitHub Pages

For free hosting, use a public repository. In **Settings → Pages**, select **Deploy from a branch**, branch **main**, folder **/ (root)**, and save. The `.nojekyll` file serves the HTML without Jekyll processing.

No custom domain is required. GitHub assigns a `https://<username>.github.io/<repository>/` address and updates it when changes reach `main`.

## Edit

Edit `index.html` directly. Translations live in the `textos` JavaScript object. Each language has ten questions with three alternatives. The shared `corretas` array contains the correct answer indexes, starting from zero.

## Credits

An independent recreation inspired by the [XGH axioms](https://gohorse.com.br/extreme-go-horse-xgh.html) and the original Go Horse certification experience. The Go Horse logo comes from [gohorse.com.br](https://gohorse.com.br/wp-content/uploads/2017/05/horse21.png).

Made with love, using Codex.
