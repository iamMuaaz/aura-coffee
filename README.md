# Aura Coffee | Specialty Craft Blends

A modern, visually stunning, fully accessible single-page web experience for a premium specialty coffee brand, built for the **ACM MAJU Vibe Coding Competition** (12th November 2026).

---

## 📋 Competition & Submission Details

> **Note for Judges:** This project was developed as a **Solo Submission** adhering to all competition constraints (frontend prototype only, no paid software, no database/backend, fictional sample data).

| Field | Submission Details |
| :--- | :--- |
| **Project Brief** | **Brief #8 — Coffee Brand Website** |
| **Participation Type** | **Solo Participant** |
| **Participant Name** | Muaaz Ibrahim |
| **Student ID** | FA26-BSCS-0109 |
| **Institution** | Muhammad Ali Jinnah University (MAJU) |
| **GitHub Repository** | https://github.com/iamMuaaz/aura-coffee |
| **Live Vercel Link** | https://auracoffee-two.vercel.app/ |
| **Target Audience** | Specialty coffee enthusiasts, students, and young professionals seeking ethically sourced, small-batch roasted single-origin coffee |
| **Primary User Task** | Browse curated roast collections, filter by roast level, and complete a simulated checkout order with real-time feedback |

---

## 🎯 What We Built & Requirements Breakdown

### 1. Brand Experience & Landing View
- **Luxury Intro Preloader**: A satisfying opening animation with a glowing geometric gold emblem, expanding gold progress line, and an elegant curtain dissolve into the hero section.
- **Hero Section**: High-impact dark aesthetic with Unsplash roasted bean photography, radial glow orbs, gold brand typography, headline, live animated counter metrics (*12 Origins*, *5,000 Cups Daily*, *98% Satisfaction*), and a primary `"Order Now"` call-to-action button.
- **Ambient Aroma Canvas**: An ultra-lightweight GPU-accelerated HTML5 canvas rendering 35–40 floating golden embers and coffee aroma particles drifting upwards with gentle mouse evasion.
- **Brand Story ("Our Roots")**: Comprehensive narrative explaining direct-trade partnerships with small-hold farmers in Colombia, Ethiopia, and Guatemala, ethically sourced beans, small-batch roasting, plus store hours, contact, and fictional roastery address in Lahore.
- **Signature Drinks Menu**: 6-item interactive responsive grid featuring Espresso, Caffè Latte, Cold Brew, Matcha Fusion, Mocha, and Pour Over with pricing and high-definition photography.
- **Featured Blends**: 3 product cards (*Midnight Eclipse*, *Golden Hour*, *Velvet Dawn*) with roast badges, bean metadata, interactive roast filter tabs (All / Dark / Medium / Light), and `"Add to Cart"` functionality.
- **Social Proof / Reviews**: 3 customer testimonials with star ratings and reviewer roles.
- **Roastery Store Info ("Visit Us")**: Physical address, opening hours, customer contact, free delivery guidelines, and roastery visual showcase.
- **Newsletter Subscription**: Email validation form with confirmation toast notification.
- **Footer**: Brand statement, quick links, working interactive modals for policies and social media, and mandatory competition disclaimers.

---

### 2. Interactive Features & Complete User Flow

1. **Add to Cart & Live Notification**:
   - Updates the live cart badge count in the navigation bar with bounce animation.
   - Temporarily transforms button state to `✓ Added` with feedback.
   - Triggers an animated slide-in toast notification in the top-right corner.
2. **Interactive Cart Drawer & Professional Checkout Flow**:
   - Clicking the cart icon in the navbar opens a shopping cart modal with itemized pricing, quantities, and individual `✕` item removal with live price recalculation.
   - Clicking `"Proceed to Checkout →"` transitions seamlessly to a **Professional Checkout Modal**:
     - **Customer Details**: Full Name, Phone Number, Email Address.
     - **Shipping Address**: Street Address, City Dropdown (*Lahore Local Express*, *Karachi*, *Islamabad*, *Rawalpindi*, etc.).
     - **Payment Selection**: Cash on Delivery (COD - Recommended), JazzCash / EasyPaisa (Instant), or Credit / Debit Card (Simulated Demo).
     - **Order Summary**: Subtotal, Delivery Fee (Free on orders $\ge \$25$, else $\$3.50$), and Total Amount.
     - **Simulated Order Placement**: Submitting the form triggers a loading state (`⏳ Processing Order...`), empties the cart, resets the badge, and renders a **Complete Order Confirmation Receipt** with an assigned Order Reference Number (`#AC-XXXXX`), customer summary, delivery address, and estimated timeline.
3. **Product Roast Filter Tabs**:
   - Filter buttons (All / Dark / Medium / Light) dynamically show or hide cards in the DOM.
4. **Interactive Policy Modals**:
   - **Shipping**: Local Lahore delivery tiers, domestic rates, international DHL Express estimates, tracking, and returns.
   - **Privacy Policy**: GDPR-inspired privacy practices, data collection, and rights.
   - **Terms & Conditions**: 7 structured legal clauses adapted for an e-commerce demo.
5. **Interactive Social Media Previews**:
   - Clicking Instagram, Twitter / X, or Facebook opens preview dialogs with verified handles, follower statistics, and fictional community notes.
6. **Smooth Scrolling & Back-to-Top**:
   - Smooth CSS scroll behavior for all navigation anchors.
   - Top Glowing Gold Scroll Progress Bar tracking scroll depth from 0% to 100%.
   - Floating back-to-top button that fades in once scrolled past 500px.
   - ScrollSpy active link tracking in the navigation bar.

---

## ♿ Accessibility & Quality Verification

| Accessibility Feature | Implementation Detail |
| :--- | :--- |
| **Keyboard Focus** | Explicit `:focus-visible` CSS rule applying a 2px solid gold (`#c9a96e`) outline with 3px offset across all links, buttons, and inputs. |
| **Color Contrast** | High-contrast palette: Cream text (`#f7f4ee`) and brightened muted text (`#bab4c4`) over dark background (`#09080d`) exceeding WCAG AAA standards (> 15:1 ratio). |
| **Semantic HTML5** | Meaningful landmark tags: `<nav>`, `<header>`, `<main>`, `<section>`, `<article>`, `<button>`, `<footer>`. |
| **Image Descriptions** | Every `<img>` includes comprehensive, descriptive `alt` attributes explaining roast style, origin, or drink preparation. |
| **ARIA Attributes** | Accessible labels (`aria-label`), dialog metadata (`aria-modal`, `role="dialog"`), live region (`aria-live="polite"`), and tablist roles (`role="tablist"`, `aria-selected`). |
| **Mobile Responsiveness** | Fully tested and optimized with responsive CSS media queries down to 320px mobile screens, including collapsible hamburger navigation. |

---

## 🤖 AI Usage & Purposeful Iteration Disclosure

- **AI Tools Used**: Antigravity (Claude / Gemini).
- **Categories of Assistance**: Rapid UI scaffolding, responsive CSS layout, design token planning, copywriting, and interactive modal state architecture.
- **Human Verification & Manual Edits**:
  - Replaced standard native `alert()` with a custom accessible toast notification system and multi-step cart drawer.
  - Replaced emoji with custom Geometric Gold Coffee Cup SVG vector branding and added a crisp SVG favicon for the browser tab.
  - Designed a complete checkout workflow taking user shipping details, payment preferences, and generating order receipts.
  - Added `:focus-visible` keyboard accessibility styling across all interactive elements.
  - Engineered an ultra-lightweight GPU particle canvas for floating ambient embers.
  - Verified color contrast ratios for dark mode accessibility.
  - Tested mobile navigation toggling and keyboard escape handlers on modals.

---

## 📦 Fictional Sample Data Notice

All sample data used across this website is strictly **fictional** and created solely for the ACM MAJU Vibe Coding Competition:
- Brand name "Aura Coffee" is fictional.
- Product names, descriptions, prices, and reviews are fictional.
- Store address (*42 Ember Lane, Gulberg III, Lahore*), phone, and email are fictional.
- No real transactions, personal user data, or payments are processed.

---

## 🎨 Asset Credits & Licenses

| Asset | Source / Creator | License |
| :--- | :--- | :--- |
| **Typography** | [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) & [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts | SIL Open Font License (OFL) |
| **Photography** | High-resolution specialty coffee photography via [Unsplash](https://unsplash.com) | Unsplash Free Commercial License |
| **Vector Icons** | [Heroicons](https://heroicons.com) by Tailwind Labs & Custom SVG Vector Paths | MIT License |

---

## ⚠️ Limitations & Future Enhancements

- **Current Limitations**: Frontend-only static prototype (no persistent database or live payment gateway integration).
- **Future Enhancements**: Integration with a headless CMS for live bean catalog updates, live brewing guide calculator, and customer account dashboard.

---
*Created for the ACM MAJU Vibe Coding Competition — 12th November 2026.*
