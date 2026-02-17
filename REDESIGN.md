# VitaVault Website Redesign — Light Theme, Premium Health Feel

## The Problem
Current site looks like ScanWow (dark, techy, Claude-esque). VitaVault is a HEALTH app — it needs to feel clean, bright, trustworthy, and premium. Think Apple Health meets Calm meets Oura Ring's marketing.

## Design Direction

### Color Palette
- **Background**: Clean white (#FFFFFF) with very subtle warm gray sections (#F8FAFB or #F0F4F5)
- **Primary accent**: Teal (#0D9488 / #14B8A6) — matches the app
- **Secondary accent**: Soft purple (#8B5CF6) — for AI/Coach features only
- **Text**: Dark charcoal (#1A1A2E or #111827) — NOT pure black
- **Muted text**: Medium gray (#64748B)
- **Cards**: White with subtle shadow and light border (#E2E8F0 border, soft shadow)
- **Gradients**: Very subtle — teal-to-mint for hero backgrounds, NOT dark gradients

### Typography
- System font stack (SF Pro on Apple, system-ui elsewhere)
- Large, confident headings with tight letter-spacing
- Generous whitespace — let it breathe

### Visual Style
- **Light and airy** — lots of white space
- **Soft shadows** instead of borders where possible
- **Rounded corners** (16-20px on cards)
- **Subtle gradient backgrounds** on sections (white → very light teal/mint)
- **NO dark sections** — everything stays light
- **Health iconography** — hearts, shields, pulse lines as decorative elements
- Think: Apple's product pages, Oura Ring, Whoop's marketing site, Linear.app (but light)

### Hero Section
- Clean white/light mint gradient background
- Maybe a subtle radial glow behind the phone mockup
- The phone mockup should show a DARK screen (like the actual app) against the light background — creates nice contrast
- Badge should be subtle (light teal background, dark teal text)

### Cards
- White background, subtle shadow (0 2px 12px rgba(0,0,0,0.06))
- Light border (1px solid #E2E8F0)  
- Teal icon/accent per card
- Clean, minimal — not heavy

### Pricing Section  
- Cards with very subtle teal gradient border for the featured one
- Clean checkmarks in teal
- "No subscription" callout in a soft teal banner

### Navigation
- White/frosted glass sticky nav
- Clean logo + links
- Teal "Download" button

### Footer
- Light gray background (#F1F5F9)
- Standard footer links

## Pages to Rebuild

### index.html (Landing Page)
Keep all the same CONTENT from the current site but completely restyle:
- Nav, Hero (with badge, h1, subtitle, buttons, phone mockup)
- Features (6 cards in grid)
- How It Works (3 steps)  
- Pricing (Free vs Premium)
- CTA section
- Footer

### developers/index.html
Keep all the same CONTENT but restyle:
- The code blocks should still be dark (dark code blocks on light page look great)
- Cards and layout go light
- Keep copy-to-clipboard functionality

### privacy/index.html and terms/index.html
- Light theme versions

### assets/favicon.svg
- Keep current (it works on both light and dark)

## Technical Notes
- Pure HTML/CSS, minimal JS (mobile nav toggle, smooth scroll, copy buttons)
- Mobile responsive
- Keep all SEO meta tags, OG tags, canonical URLs
- Keep all links and content the same
- Just completely restyle from dark → light premium health aesthetic

## Reference Sites for Inspiration
- Apple Health marketing pages
- oura.com
- whoop.com
- calm.com
- linear.app (for clean light UI patterns)
- arc.net

## When Done
Stage and commit all changes with message: "redesign: light premium health theme"
