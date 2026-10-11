# Qiyao Flashlight — B2B Export Website

Single-page English-first marketing website for **Huizhou Qiyao Electronic Technology Co., Ltd.**
(OEM / ODM manufacturer of LED flashlights, headlamps and portable outdoor lighting).

## Structure

```
.
├── index.html      # entire site: inline CSS + JS, EN / ZH language toggle
├── images/         # 8 product images (1200x711 JPEG, progressive)
└── .nojekyll       # serve files as-is, skip Jekyll processing
```

No build step, no dependencies, no external CDN. Open `index.html` directly, or serve the
folder with any static host.

## Sections

Hero · Products (flashlights + outdoor & portable lighting) · OEM / ODM process ·
About · Why Us · Certification & compliance · Contact form

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Contact form

The form has no backend. It composes a `mailto:` link and opens the visitor's mail client.
The destination address is a single constant near the top of the `<script>` block:

```js
var CONTACT_EMAIL = "your-email@example.com";
```

**Replace it with the real business address before going live.**

## Before public promotion

- [ ] Replace the placeholder email and phone / WhatsApp number shown with orange dashed
      underline on the page.
- [ ] Confirm the certification badges (CE / RoHS / UN38.3) reflect certificates actually
      held, and delete any that do not.
- [ ] Swap the AI-generated product images for real product photography. They are
      placeholders, not photographs of our own products.
- [ ] Review the marketing claims (factory-direct, batch inspection, in-house tooling) and
      keep only what is accurate.

## License

All rights reserved. Content, copy and imagery belong to Huizhou Qiyao Electronic
Technology Co., Ltd.
