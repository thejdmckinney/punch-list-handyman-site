# Assets Checklist

## Required Image Files

### 1. Logo
- **Filename:** `logo.svg`
- **Location:** `/assets/img/logo.svg`
- **Dimensions:** Flexible (SVG scales), recommend 200×50px artboard
- **Format:** SVG (vector)
- **Usage:** Header navigation on all pages
- **Design Notes:** Should work on white backgrounds; incorporate brand colors (charcoal #2d3748, electric blue #0066ff, safety orange #ff6b35)

### 2. Favicon
- **Filename:** `favicon.ico`
- **Location:** `/favicon.ico` (root directory)
- **Dimensions:** 32×32px (standard), multi-resolution ICO recommended
- **Format:** ICO file with 16×16, 32×32, 48×48 sizes
- **Usage:** Browser tab icon
- **Design Notes:** Simple icon from logo mark; should be recognizable at small size
- **Optional:** Add `favicon-16x16.png`, `favicon-32x32.png`, `apple-touch-icon.png` (180×180) for better cross-platform support

### 3. Open Graph Image
- **Filename:** `og-knockout.png`
- **Location:** `/assets/img/og-knockout.png`
- **Dimensions:** 1200×630px (required for Facebook/LinkedIn/Twitter)
- **Format:** PNG or JPG
- **Usage:** Social media preview cards when site is shared
- **Design Notes:** 
  - Include brand name "Punch List Handyman"
  - Tagline: "One Visit. Everything Done."
  - Service area: "Dallas–Fort Worth"
  - Use brand colors with strong contrast
  - Keep text readable at small sizes
  - Avoid placing critical content in outer 10% (may be cropped)

### 4. Service Area Map
- **Filename:** `dfw-map.png`
- **Location:** `/assets/img/dfw-map.png`
- **Dimensions:** 600×400px recommended (responsive, so flexible)
- **Format:** PNG or JPG
- **Usage:** `/service-area.html` page only
- **Design Notes:** 
  - Simple map showing Dallas–Fort Worth metro area
  - Mark major cities served (Dallas, Fort Worth, Plano, Frisco, Arlington, etc.)
  - Use brand colors for markers/highlights
  - Clean, minimal design (not cluttered)
- **Alternative:** Can use Google Maps embed instead (instructions in service-area.html comments)

---

## Assets Summary

| File | Path | Size | Format | Priority |
|------|------|------|--------|----------|
| `logo.svg` | `/assets/img/logo.svg` | ~200×50px | SVG | **CRITICAL** |
| `favicon.ico` | `/favicon.ico` | 32×32px | ICO | **CRITICAL** |
| `og-knockout.png` | `/assets/img/og-knockout.png` | 1200×630px | PNG/JPG | **HIGH** |
| `dfw-map.png` | `/assets/img/dfw-map.png` | 600×400px | PNG/JPG | Medium |

---

## Implementation Status

- [ ] `logo.svg` - Replace placeholder in header
- [ ] `favicon.ico` - Add to root directory, add `<link>` tag to `<head>` if using PNG alternatives
- [ ] `og-knockout.png` - Replace placeholder referenced in all page `<meta property="og:image">` tags
- [ ] `dfw-map.png` - Add to `/assets/img/` OR configure Google Maps embed in service-area.html

---

## Additional Notes

- **Logo Usage:** Currently referenced in all HTML pages via `<img src="/assets/img/logo.svg" alt="Punch List Handyman">`
- **OG Image Usage:** Referenced in `<meta property="og:image">` and `<meta name="twitter:image">` tags on all pages
- **Map Alternatives:** If using Google Maps embed instead of static image, delete the `<img>` placeholder in service-area.html and uncomment the `<iframe>` code
- **No Stock Photos Needed:** Site design uses brand colors and typography—no decorative imagery required
- **Keep It Minimal:** These 4 assets are sufficient for the entire site

---

## Quick Add: Favicon to HTML

If you create PNG favicons instead of/in addition to favicon.ico, add these to the `<head>` of all HTML pages:

```html
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
```

For `.ico` only:
```html
<link rel="icon" href="/favicon.ico">
```
