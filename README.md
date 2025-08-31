# Kii-X Exchange — Crypto Landing Page

A responsive, multi-section landing page for a crypto exchange built with **Bootstrap**, **HTML5**, **CSS3**, and **basic JavaScript**. It includes animated hero sections, sticky navbar, “back to top” behavior, feature cards, a sample markets table, social links, and reusable PHP partials for header and footer.

> **Note:** This project is a **front-end demo**. It does not process payments, execute trades, or connect to real exchange APIs.

---

## Key Features

- Responsive layout with Bootstrap 5
- Animated UI with WOW.js + Animate.css
- Sticky navbar with shadow on scroll
- Spinner/splash loader
- Back-to-top button with smooth scroll
- Feature grid and CTA blocks
- Sample market table for coins/metrics
- Social section with icon buttons
- Modular PHP includes: `header.php`, `footer.php`
- Organized styles across multiple CSS files

---

## Tech Stack

| Layer         | Tools / Libraries                                                                 |
|---------------|------------------------------------------------------------------------------------|
| UI Framework  | Bootstrap 5                                                                        |
| Icons         | Font Awesome 5, Bootstrap Icons                                                    |
| Animations    | WOW.js, Animate.css                                                                |
| JS Utilities  | jQuery, jQuery Easing, Waypoints, CounterUp, Owl Carousel                          |
| Fonts         | Google Fonts (Open Sans, Roboto)                                                   |
| Build/Server  | PHP includes (optional), PHP built-in server for local dev                         |

---

## Project Structure 
```
project/
├─ index.php # main page (uses header/footer includes)
├─ header.php # navbar / header partial
├─ footer.php # footer partial
├─ css/
│ ├─ bootstrap.min.css
│ ├─ style.css # general styles
│ ├─ estilos.css # custom components
│ └─ tabla.css # table-specific styles
├─ scss/
│ ├─ bootstrap/scss
│ └─ bootstrap.scss
├─ js/
│ └─ main.js # spinner, sticky nav, back-to-top, WOW init
├─ lib/ # third-party libraries (wow, owlcarousel, etc.)
├─ img/ # images (hero, icons, social, etc.)
```
## Getting Started

### 1) Clone the repository
```bash
git clone [https://github.com/ScarletRot0/kii-x-exchange.git](https://github.com/ScarletRot0/cryptoKX.git)
cd cryptoKX
```
### 2) Serve locally
Because the page uses PHP includes (header.php, footer.php), the simplest way to run it is the PHP built-in server:
```bash
php -S localhost:8000
```
Then open: http://localhost:8000/index.php

## Configuration & Customization
 * Branding & Text: Edit copy in index.php and partials in header.php / footer.php.
 * Colors & Theme: Adjust variables/classes in:
 * css/style.css (global styles)
 * css/estilos.css (custom sections/components)
 * css/tabla.css (markets table)
 * Images: Replace assets in /img (hero images, icons, logos, social icons).
 * Fonts: Tweak Google Fonts in the <head> of index.php.
 * Libraries: CDN links are in the <head> and before </body>. If you self-host, place them under /lib and update paths.

## Accessibility and SEO (quick wins)

 * Add descriptive alt text for images.
 * Use semantic headings (H1, H2, H3).
 * Optimize meta tags: title, description, og:*, twitter:*.
 * Ensure sufficient color contrast (buttons, text over images).
 * Minify CSS/JS for production and lazy-load heavy assets.

## Security Notice
This is not a real exchange. Do not collect credentials, process payments, or claim financial services without implementing proper backend, security, compliance (KYC/AML), and legal review.

