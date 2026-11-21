# ☕ Mocha Café & Roastery — Jaipur

A complete UI/UX redesign of the **Mocha Café & Roastery** website in **C-Scheme, Jaipur**. Built purely with semantic **HTML5** and **Tailwind CSS**, featuring dark mode support via Tailwind (`dark:`), FontAwesome CDN vector icons, responsive layouts across mobile, tablet, and desktop, and clean typography.

---

## 🎨 Design System & Highlights

- **Typography System (2 Font Families)**:
  - **Headings**: `Playfair Display` (editorial serif for warmth, craftsmanship, and elegance).
  - **Body & UI**: `Plus Jakarta Sans` (modern, legible sans-serif with comfortable line-height across all devices).
- **Color Palette**:
  - **Light Mode**: Warm cream background (`#FAF7F2`), surface cards (`#FFFFFF`), roast terracotta accents (`#B35E32`), deep espresso text (`#281A12`).
  - **Dark Mode (`dark:`)**: Roasted espresso background (`#120E0B`), warm dark surfaces (`#1A1410`), glowing amber terracotta (`#E27D48`), warm ivory text (`#F4ECE3`).
- **Vector Icons**: FontAwesome 6.5.1 CDN vector icons (`fa-solid`, `fa-brands`).
- **Zero JavaScript**: Pure HTML & Tailwind CSS. The mobile navigation menu functions with a pure CSS checkbox hack (`#nav-toggle` with `peer-checked:flex`). Zero JavaScript files, zero inline event handlers.
- **Strict Semantic HTML**:
  - Exactly **one `<header>`** and **one `<footer>`** per page.
  - Proper heading hierarchy with exactly **one `<h1>` per page**.
  - Semantic tags throughout: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, and `<address>`.
  - Meaningful, descriptive `alt` text on every single image for accessibility and SEO.
  - Clean, unbloated markup without unnecessary ARIA tags.
- **Social Media Integration**:
  - Social icons (Instagram, Facebook, X, WhatsApp, TripAdvisor) with `href="#"` located in both header and footer.
- **Layout & Responsiveness**:
  - Both Flexbox and CSS Grid used meaningfully across major sections.
  - Mobile-first approach optimized for **Mobile (~375px)**, **Tablet (~768px)**, and **Desktop (~1280px)**.
  - Zero horizontal overflow at any viewport width.

---

## 📄 Pages & Sections

### 1. Home (`index.html`)
- **Header & Navigation**: Sticky header with logo, navigation links, social icons, and a "Book a Table" CTA button.
- **Hero Section (CSS Grid)**: Jaipur C-Scheme badge, main heading, dual CTAs, craft statistics (100% Arabica, 48hr roast cycle, 7 AM bakery), and courtyard photography with review rating badge.
- **Core Craft Strip**: 4-column feature grid (Single-origin beans, micro-batch roasts, pure butter bakery, courtyard sanctuary).
- **Signature Creations**: Bestseller items with pricing, imagery, and flavor notes (Sea-Salt Caramel Mocha, Chikmagalur V60, French Butter Croissant).
- **Roasting Philosophy & Story**: Dual-photo grid highlighting direct trade sourcing, SCA 84+ cupping score, and custom roast profiles.
- **The Courtyard Experience**: Ambiance features including high-speed WiFi for remote work, pet-friendly seating, and warm evening lighting.
- **Community Testimonials**: Customer reviews with reviewer avatars, star ratings, and quotes.
- **Farm-to-Cup Journey**: 4-step process (Harvest, Micro-Roast, Extraction, Courtyard Sip).
- **Hours & Location Strip**: Quick visit details with directions link and table reservation button.
- **Global Footer**: Brand story, quick links, operating hours, contact address, and social links (`href="#"`).

### 2. Menu (`menu.html`)
- **Menu Hero & Quick Jump Navigation**: Jump-link pills for `#espresso`, `#slow-bar`, `#bakery`, `#beans`, and `#customizations`.
- **01 / The Espresso Bar (CSS Grid)**: Sea-Salt Caramel Mocha, Spanish Cortado, Classic Flat White, Citrus Espresso Tonic.
- **02 / Slow Extraction Bar (CSS Grid)**: Chikmagalur V60, 18-Hour Reserve Cold Brew, Dialed Espresso Flight, Cascara Cherry Brew.
- **03 / Fresh From The Oven (CSS Grid)**: French Butter Croissant, Almond Pain au Chocolat, Avocado & Feta Sourdough Toast, Pistachio Kouign-Amann.
- **04 / Take-Home Coffee Beans (CSS Grid)**: Jaipur Morning Roast, Chikmagalur Honey Micro-Lot, Roaster’s Trio Box with grind customization.
- **05 / Customizations & Equipment Notes (CSS Grid)**: Plant-based milks (Oat, Almond, Soy), EK43 custom grinds, and bakery pre-orders.
- **Pre-Footer CTA Banner & Footer**.

### 3. Gallery (`gallery.html`)
- **Gallery Hero**: Introduction to the visual ambiance of Mocha Jaipur.
- **Pure Visual Photo Exhibition (CSS Grid)**:
  - 12 curated moments displayed in clean, unobstructed `<figure>` frames with smooth hover zoom (`group-hover:scale-105`) and elevated card shadows (`hover:shadow-2xl`).
  - **Photo-First Design**: All text overlays, badges, and dark gradient scrims have been removed so the photography remains the sole, clear focus.
  - Covers manual V60 extraction, courtyard arches, roastery machinery, golden espresso crema, fresh morning pastries, evening lighting, cold brew, latte art, roastery lounge, and artisan bakes.
- **Gatherings & Community Section**: Weekend coffee cuppings, private courtyard bookings, and acoustic music evenings.
- **Pre-Footer CTA Banner & Footer**.

### 4. Contact & Reservations (`contact.html`)
- **Contact Hero**: Page introduction and greeting.
- **Equal-Height Reservation & Details Section (CSS Grid)**:
  - **Table Booking & Orders Card (`lg:col-span-7`)**: Fully accessible reservation form with every input linked to its corresponding `<label for="...">`, correct input types (`text`, `tel`, `email`, `date`, `time`, `<select>`, `<textarea>`), and submit action.
  - **Find Us in Jaipur Card (`lg:col-span-5`)**: Detailed address, direct phone link, email, opening hours, and live open status badge.
  - **Balanced Heights**: Both cards use `flex flex-col justify-between` and CSS Grid column stretching to maintain the **exact same height** on tablet and desktop screens.
- **Full-Width Interactive Map**:
  - The Google Maps `<iframe>` is placed in its own dedicated section outside the reservation grid, spanning **100% full viewport width** edge-to-edge with responsive heights (`h-[400px] sm:h-[480px] lg:h-[540px]`) and a floating navigation card.
- **Neighborhood & Transit Strip**: Transit times from Civil Lines Metro, valet parking details, Central Park proximity, and pet policies.
- **Visitor Guide & FAQ Grid**: 4 cards answering questions about walk-in tables, remote work amenities, pets, and home bean grinding.
- **Pre-Footer CTA Banner & Footer**.

---

## 📁 Project Structure

```
mocha/
├── assets/
│   ├── icons/
│   │   ├── favicon.ico
│   │   └── icon.svg
│   └── images/
│       ├── 18-coldbrew.png
│       ├── almond-pain-chocolat.png
│       ├── ananya.png
│       ├── avocado-sourdough.png
│       ├── classic-flat-white.png
│       ├── coldbrew.png
│       ├── courtyard.png
│       ├── croissant.png
│       ├── espresso-extraction.png
│       ├── evening.png
│       ├── hero-jaipur.png
│       ├── mocha-latte-jaipur.png
│       ├── pastry.png
│       ├── roaster.png
│       ├── rohan.png
│       ├── spanish-cortado.png
│       ├── tonic.png
│       ├── v60-extraction.png
│       ├── v60.png
│       └── vikram.png
├── contact.html     # Reservations, contact information, and full-width map
├── gallery.html     # Pure visual photo exhibition and community gatherings
├── index.html       # Landing page, craft highlights, story, and testimonials
├── menu.html        # Espresso bar, slow bar, bakery, and take-home beans
└── README.md        # Project documentation
```

---

## 🚀 How to Run Locally

Open any of the HTML files directly in your web browser, or serve them locally using any static web server:

```bash
# Using Python
python -m http.server 3000

# Using Node.js (npx serve)
npx serve .
```

Then visit `http://localhost:3000` in your browser.
