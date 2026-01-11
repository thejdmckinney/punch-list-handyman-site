# Punch List Handyman

## 🧠 MASTER COPILOT PROMPT

*(Paste this at the top of your main project or before starting a new file)*

You are assisting in building a lean, static, conversion-focused website for a productized home service called Punch List Handyman.

This site is intentionally minimal. Do NOT add features, pages, scripts, animations, forms, or content that are not explicitly requested.

### CORE CONSTRAINTS (NON-NEGOTIABLE)

- Static site only (GitHub Pages compatible)
- HTML + CSS + minimal vanilla JS only
- No frameworks, no build tools, no CMS
- No blogs, no FAQs, no galleries, no testimonials unless explicitly requested
- No dynamic pricing, no calculators, no custom booking logic

### BUSINESS MODEL CONTEXT

Punch List Handyman offers one product:

A one-visit, time-based punch list service

Two pricing tiers only:
- **Half-Day Knockout™** — $495 (3–4 hours)
- **Full-Day Knockout™** — $895 (6–8 hours)

Customers are buying closure, not labor.

### PRIMARY GOAL OF THE WEBSITE

- Make the concept instantly clear
- Set firm expectations
- Funnel qualified users to an external booking system (Calendly/TidyCal + Stripe)

### SITE MAP (DO NOT ADD PAGES)

The site consists of exactly these pages:
- `index.html` (Home)
- `book.html` (Booking overview + outbound CTA)
- `pricing.html`
- `what-fits.html`
- `service-area.html`
- `privacy.html`
- `terms.html`

### DESIGN & UX RULES

- Clean, authoritative, professional
- "Clipboard authority" aesthetic
- No gimmicks, no fluff, no marketing hype
- Clear hierarchy, generous whitespace
- Mobile-first, responsive

### BRAND TONE

- Confident
- Direct
- Calm
- Decisive

Avoid casual language, emojis, jokes, or slang.

### HEADER & FOOTER RULES

**Header:**
- Logo (left)
- Navigation: Home | Pricing | What Fits | Book
- Primary CTA button: "Book My Knockout"

**Footer:**
- Service area (Dallas–Fort Worth)
- Business name
- Privacy & Terms links
- No social media links

### BOOKING LOGIC (IMPORTANT)

- Do NOT build a booking system
- All "Book" CTAs link to an external scheduling page
- The website's role is education and qualification only

### SEO REQUIREMENTS

- Semantic HTML
- One H1 per page
- Clear H2/H3 structure
- Meta title and description included in each page
- Local SEO focus on Dallas–Fort Worth

### OUTPUT RULES

- Only generate code or copy that directly supports the above
- If unsure, ask for clarification instead of inventing
- Never introduce extra sections or features "for best practice"
- Build strictly within these constraints.


## Project Structure
```
/
├── .github/
│   └── copilot-instructions.md
├── assets/
│   ├── css/
│   │   └── styles.css
│   └── img/
│       ├── logo.svg
│       └── og-image.png
├── index.html
├── book.html
├── pricing.html
├── what-fits.html
├── privacy.html
├── terms.html
├── HEADER-FOOTER-SNIPPET.html
└── README.md
```

## Brand Identity

**Colors:**
- Charcoal: `#2d3748` (primary text)
- White: `#ffffff` (backgrounds)
- Electric Blue: `#0066ff` (primary CTA, accents)
- Safety Orange: `#ff6b35` (secondary accents)

**Aesthetic:**
- "Clipboard authority" design
- Clean, calm, decisive
- Generous whitespace
- Strong typography
- Checkmark/list visual motifs
- Subtle 2px borders

**Tone:**
- Confident
- Direct
- No gimmicks or marketing hype
- Avoid casual language, emojis, jokes, slang

## Pages

- **index.html** - Homepage
- **book.html** - Booking overview with external CTA to {{BOOKING_URL}}
- **pricing.html** - Two packages: Half-Day Knockout™ ($495) and Full-Day Knockout™ ($895)
- **what-fits.html** - Service scope with clear inclusions/exclusions
- **privacy.html** - Privacy policy
- **terms.html** - Terms of service

## Key Components

### Header Navigation
- Logo (left)
- Nav links: Home | Pricing | What Fits | Book
- Primary CTA button: "Book My Knockout" → {{BOOKING_URL}}
- Mobile-responsive with hamburger toggle

### Footer
- "Serving Dallas–Fort Worth"
- Business name
- Privacy & Terms links
- No social media links

### CSS Utilities
- `.btn-primary` - Electric blue button
- `.btn-secondary` - Safety orange button
- `.checklist` - Checkmark list items
- `.exclusion-list` - X-mark list items
- `.card` - Bordered content card
- `.card-highlight` - Featured card with "MOST POPULAR" badge
- `.container` - Max-width 1100px container
- `.two-col` - Two-column responsive grid

## Implementation Notes

1. **Booking System**: All "Book" CTAs link to `{{BOOKING_URL}}` - replace this placeholder with your actual Calendly/TidyCal/Stripe URL

2. **Header/Footer**: Consistent across all pages. See `HEADER-FOOTER-SNIPPET.html` for copy-paste template

3. **Mobile Navigation**: Simple JavaScript toggle for mobile menu (< 768px)

4. **SEO**: Each page has semantic HTML, one H1, meta descriptions, and local SEO focus on Dallas-Fort Worth

5. **Static Only**: No frameworks, no build tools, no server-side logic

---

Professional handyman services website built with HTML and CSS.
