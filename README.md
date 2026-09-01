# Developer Broadsheet Portfolio

A unique, typography-driven personal portfolio designed to emulate the look and feel of a vintage newspaper broadsheet. It relies entirely on structural rules, distinct type contrast, and monochrome ink to deliver a highly readable, editorial experience.

## ✨ Features

- **Vintage Typography System:** Uses a high-contrast serif (Playfair Display) paired with a heavy condensed grotesque-sans (Anton) and a wide-tracked structural font (Public Sans).
- **Responsive Layout:** 
  - On desktop, it renders a dense, print-like three-column grid.
  - On mobile, it intelligently reflows to a vertical reading experience while maintaining the newspaper structural rules.
- **PWA & Offline Support:** Equipped with a `stale-while-revalidate` Service Worker (`sw.js`) to instantly load assets from the cache, enabling fast load times and seamless offline capabilities.
- **Optimized Media:** Uses WebP images and a "blur-up" loading pattern for the portrait image to improve performance.
- **Comprehensive SEO:** Includes standard meta tags, Open Graph properties for rich social sharing, Twitter Cards, and appropriately sized favicons for all devices.
- **Zero Build-Step:** Pure HTML, JavaScript, and Tailwind CSS via CDN. No complex build tools required.

## 🚀 Getting Started

Since this is a static site without a build process, getting started is extremely easy.

1. Clone or download this repository.
2. Open `index.html` in your browser, or serve it using any simple local HTTP server:
   ```bash
   python3 -m http.server 8000
   # or
   npx serve .
   ```
3. Visit `http://localhost:8000` to view the broadsheet.

## 📝 Customization

All portfolio content is abstracted into a single JavaScript configuration object inside `index.html`. 

To update the content with your own:
1. Open `index.html`.
2. Locate the `portfolioData` object inside the `<script>` tag.
3. Edit the properties (meta, contact, skills, projects, achievements, education) as needed. The DOM will automatically render your updated content!

To update the portrait image:
1. Replace `profile-pic-vintage.webp` with your own image.
2. Replace `profile-pic-vintage-lowres.webp` with a heavily scaled-down version (e.g., 32x32) of your image for the blur-up loading effect.

## 🛠 Tech Stack

- HTML5 / Vanilla JavaScript
- [Tailwind CSS](https://tailwindcss.com/) (via CDN)
- [Google Fonts](https://fonts.google.com/) (Playfair Display, Anton, Public Sans)
- Service Workers API

## 📜 License

MIT License. Free to use, modify, and distribute for your own personal portfolios!
