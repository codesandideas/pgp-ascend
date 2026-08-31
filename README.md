# PGPx Ascend — landing page

Static landing page for **PGPx Ascend: AI & Product Building**, an 8-month
part-time program at Mesa School of Business for working professionals.

Live at <https://mesaschool.co/pgp-ascend/>.

## Contents

```
index.html                       the whole page (inline CSS + one inline script)
wp-content/uploads/2026/02/      hero logo strips (shared with the rest of mesaschool.co)
wp-content/uploads/2026/08/      Ascend photography and guest VC logos
```

The page is self-contained apart from Google Fonts (Manrope, Instrument Serif).
There is no build step: `index.html` is the deployable artifact.

## Asset paths

Image `src` values are relative (`wp-content/uploads/...`), so the page renders
from any location: the document root of mesaschool.co, a subpath such as GitHub
Pages, a local static server, or straight off the filesystem.

```sh
python3 -m http.server 8000   # then open http://localhost:8000/
```

## Images

Photography is resized to 1600px (2000px for full-width slots), EXIF stripped,
encoded as WebP q80. Logos are WebP with alpha. The whole image set is ~1.4 MB.

## Outstanding placeholders

Slots still showing the dashed `IMAGE` placeholder, pending source files:

- 8 mentor portraits and 8 mentor company logos (card text is still `[Mentor name]`)
- 8 VC logo slots inside the mentor cards
- 5 product screenshots (automation dashboard, agent output, web app with login,
  Product Hunt launch page, B2B invoicing dashboard)
- video poster
- campus exterior / evening wide shot
