# Whitepace - SaaS Landing Page Clone

Task #06 - Frontend Development Internship (FentixTech)
Developed by: **Muhammad Afaq**
Deadline: 30 July 2026

## About this project

This is a clone of the **Whitepace - SaaS Landing Page (Community)** Figma design, built
using **pure Bootstrap 5** as required by the task. It's a project-management SaaS landing
page with a hero section, feature blocks, pricing plans, sponsor logos, testimonials, and a
footer CTA.

Reference design:
https://www.figma.com/design/YwqFjwVcT2ki1rv4iuFzG8/Whitepace---SaaS-Landing-Page--Community-

> Note: I didn't have login access to the Figma file, so this was built from the shared
> screenshots (section layout, headings, and colors) rather than exact pixel measurements.
> If you open the file yourself, double-check exact hex codes, font sizes, and spacing
> against the CSS variables below and adjust as needed.

## Tech used

- HTML5
- Bootstrap 5.3.3 (via CDN) - all layout, grid, and spacing
- Bootstrap Icons 1.11.3 (via CDN)
- Google Fonts - Poppins (headings) and Inter (body text)
- Custom CSS - only for brand colors, fonts, and the dot/network graphic
  (things Bootstrap utility classes can't express)

## Project structure

```
whitepace/
├── index.html          # Main landing page (all sections)
├── css/
│   └── style.css        # Brand colors, fonts, custom components
└── README.md            # This file
```

## Sections included (in order)

1. Navbar - logo, nav links, "Get Started" button
2. Hero - "Get More Done with whitepace"
3. Project Management - feature block with placeholder image
4. Work together - feature block with dot/network graphic
5. Use as Extension - dark navy section
6. Customise it to your needs
7. Choose Your Plan - 3 pricing cards ($9.99 / $19.99 / $49.99)
8. 100% your data
9. Our sponsors - Apple, Microsoft, Slack, Google icons
10. Work with Your Favorite Apps Using whitepace - dark navy section
11. What Our Clients Says - 3 testimonial cards
12. Try Whitepace today - closing CTA + footer

## How to run it

No build step needed - it's a static site.

1. Download/clone the `whitepace` folder
2. Open `index.html` directly in any browser

   OR, to serve it locally (recommended so relative CSS paths always resolve):

   ```
   cd whitepace
   python3 -m http.server 8000
   ```

   Then visit `http://localhost:8000` in your browser.

## Responsiveness

Built mobile-first using Bootstrap's grid breakpoints:

- Mobile (< 768px): single column, stacked sections
- Tablet (768px - 992px): 2-column grids where applicable
- Desktop (> 992px): full 2-column feature rows, 3-column pricing/testimonials

Tested by resizing the browser window and using Chrome DevTools' device toolbar.

## Customizing colors/fonts

All brand colors and fonts are defined as CSS variables at the top of `css/style.css`:

```css
:root {
  --navy: #0E1B3D;
  --sky: #BFDBFF;
  --sky-light: #EAF3FF;
  ...
}
```

Change these values in one place to re-theme the whole page.

## What I'd improve with more time

- Swap the flat placeholder blocks for the real illustrations/screenshots from the Figma file
- Match exact spacing/padding values once I have direct access to the Figma inspect panel
- Add subtle scroll-reveal animation on the feature sections
- Add a working mobile nav collapse animation test across more devices

---
Submitted for Task #06, FentixTech Frontend Internship - Muhammad Afaq
