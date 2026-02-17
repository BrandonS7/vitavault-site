# VitaVault Website — vitavault.io

## Overview
Single-page marketing site + /developers/ page for VitaVault, an iOS health data export app. Same architectural pattern as scanwow.io — static HTML/CSS, dark theme, modern design, Cloudflare Pages deployment.

## Brand
- **Name**: VitaVault
- **Tagline**: "Your Health Data. Your AI. Your Rules."
- **Accent color**: Teal (#14B8A6 / #0D9488 range — matches the app's teal accent)
- **Secondary accent**: Purple (#8B5CF6 — matches the AI insight card gradient)
- **Background**: Dark (#0B1220)
- **Cards**: (#111827)
- **Font**: System font stack (-apple-system, BlinkMacSystemFont, SF Pro, system-ui)

## Pages

### 1. index.html (Landing Page)

**Nav** (sticky top):
- Logo (text "VitaVault" with a small vault/heart icon — use SVG inline)
- Links: Features | Developers | Privacy | Download
- Download button (accent, links to App Store — use # placeholder for now)

**Hero Section**:
- Badge: "NOW ON THE APP STORE" (or "COMING SOON")
- H1: "Your Health Data. **Your AI.** Your Rules."
- Subtitle: "Export your Apple Health data in one tap. Use it with ChatGPT, Claude, Gemini — or our built-in AI Coach. Your data never touches our servers."
- Two buttons: "Download on App Store" (primary) + "View on GitHub" (secondary/outline)
- Below: a stylized phone mockup area (use a simple CSS gradient card as placeholder — we'll add screenshots later)

**Features Section** (grid of cards):
1. **One-Tap Export** — Export all your health data as JSON or CSV. Steps, sleep, heart rate, weight, workouts — everything.
2. **Your AI, Your Choice** — Feed your export into ChatGPT, Claude, or any AI. We give you the data, you choose the brain.
3. **Built-in AI Coach** — Don't want to DIY? Our AI Coach analyzes your trends, prepares doctor visit summaries, and answers health questions.
4. **Medication Tracking** — Scan pill bottle labels with your camera. AI auto-fills everything. Set reminders. Never miss a dose.
5. **Privacy First** — Your data stays on your device. Exports go to your Files app. No accounts, no cloud sync required.
6. **Open Source Format** — Our export format is fully documented and open source. Build your own tools, integrations, or dashboards.

**How It Works Section** (3 steps):
1. Connect to Apple Health (icon: heart + shield)
2. Choose your data & export (icon: download arrow)
3. Use with any AI or our Coach (icon: brain/sparkle)

**Pricing Section**:
- Free tier: Export data (JSON/CSV), view dashboard, 7-day trends
- Premium (one-time $4.99): AI Coach, medication tracking, auto-sync, all health metrics, label scanning
- Emphasize: "No subscription. Pay once, own it forever."

**CTA Section**:
- "Take Control of Your Health Data"
- Download button
- "Open source. Privacy-first. No data hostage."

**Footer**:
- VitaVault © 2026 Starboard Investments
- Links: Privacy Policy | Terms of Service | Developers | GitHub | Contact
- Email: support@vitavault.io

### 2. developers/index.html (Developer Page)

**Nav**: Same as main site, with "Developers" link active

**Hero**:
- Badge: "OPEN SOURCE"
- H1: "Build With **Your Health Data**"
- Subtitle: "VitaVault exports your Apple Health data in standard JSON and CSV formats. Use our open-source tools to feed it into any AI, database, or workflow."

**Export Schema Section**:
- Show the JSON export structure with syntax-highlighted code blocks
- Key fields: steps, heartRate, sleep, weight, activeCalories, hrv, bloodOxygen, etc.
- Example JSON snippet:
```json
{
  "exportDate": "2026-02-17T12:00:00Z",
  "deviceId": "anonymous",
  "period": "7d",
  "metrics": {
    "steps": { "total": 43133, "dailyAverage": 5719, "unit": "steps" },
    "sleep": { "lastNight": 6.7, "weeklyAverage": 7.1, "unit": "hours" },
    "heartRate": { "average": 72, "resting": 62, "unit": "bpm" },
    "weight": { "latest": 185.4, "unit": "lbs" },
    "hrv": { "average": 30, "unit": "ms" },
    "bloodOxygen": { "average": 97, "unit": "%" }
  }
}
```

**Use With Any AI Section** (cards):
1. **ChatGPT** — "Paste your export and ask: 'Analyze my health trends and give me 3 actionable recommendations'"
2. **Claude** — "Upload your JSON file and ask for a comprehensive health report"
3. **Gemini** — "Use Google AI Studio with your health data for personalized insights"
4. **Your Own App** — "Parse the JSON/CSV in Python, JavaScript, or any language. Build dashboards, alerts, or integrations."

Each card should have a code snippet or example prompt.

**GitHub Section**:
- Link to open source repo (use https://github.com/BrandonS7/vitavault-tools as placeholder)
- What's included: export schema docs, Python parsing scripts, example AI prompts, CSV converter
- "Star us on GitHub" button

**API Docs Preview** (if applicable):
- Note: "VitaVault processes all data on-device. There is no cloud API. Your data never leaves your phone unless YOU export it."
- This is a key differentiator — emphasize it

**Footer**: Same as main site

### 3. privacy/index.html
- Simple privacy policy page
- Key point: no data collection, no servers, on-device only
- Link to App Store privacy label

### 4. terms/index.html  
- Simple terms of service page

## Technical Requirements
- Pure HTML/CSS — no JavaScript frameworks, no build step
- Minimal JS only for: mobile nav toggle, smooth scroll, copy-to-clipboard on code blocks
- Responsive: mobile-first, looks great on iPhone through desktop
- Dark mode only (matches the app)
- All assets inline (SVG icons, no external dependencies)
- CSS in a single `<style>` block per page (or a shared styles.css)
- Syntax highlighting for code blocks via CSS only (colored spans)

## File Structure
```
index.html
developers/index.html
privacy/index.html
terms/index.html
assets/
  favicon.svg
  og.png (placeholder — we'll generate later)
```

## SEO
- Title tags, meta descriptions, Open Graph tags on every page
- Canonical URLs: https://vitavault.io/
- Keywords: health data export, Apple Health AI, health data privacy, open source health tools

## Deployment
- Cloudflare Pages (same as scanwow.io)
- Domain: vitavault.io

## Reference
- Style and structure based on https://www.scanwow.io and https://www.scanwow.io/developers/
- Use the same dark theme aesthetic but with teal/purple accent instead of cyan

## When Done
Commit all files with message: "feat: VitaVault website — landing page + developer docs"
