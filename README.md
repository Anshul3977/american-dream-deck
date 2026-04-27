# American Dream Meadowlands — Interactive Commercial Sales Deck

> A fully interactive, browser-based sales deck built to replace static PDFs and fragmented pitches for one of the world's largest mixed-use destinations.

**Live URL:** `statuesque-meringue-c22ac7.netlify.app`  
**Built for:** LIAT.AI Senior Frontend Engineer Assignment

---

## What This Is

A cinematic, non-linear interactive sales deck for American Dream Meadowlands — the second-largest commercial complex in the United States. Designed to close retail leasing deals, brand sponsorship packages, and event bookings without a salesperson in the room.

It functions as both a **live screen-share tool** for sales calls and a **standalone link** prospects can explore on their own.

---

## Tech Stack

| Layer | Choice | Why |
|---|---|---|
| Core | Vanilla HTML/CSS/JS | Zero build step, instant deploy, maximum performance |
| Fonts | Google Fonts (Bebas Neue, DM Sans, Playfair Display) | Display + body + serif hierarchy |
| Images | Unsplash CDN | Optimized, lazy-loaded, no self-hosting needed |
| Hosting | GitHub Pages / Netlify | Single file = trivial deploy |
| AI Tools | Claude (copy + architecture), Unsplash (visuals) | See AI section below |

No frameworks. No dependencies. No bundler. Opens in any browser instantly.

---

## Setup Instructions

### Option A — View Locally
```bash
git clone https://github.com/Anshul3977/american-dream-deck
cd american-dream-deck
open american-dream-deck.html
# or: npx serve . (if you prefer a local server)
```
### Option C — GitHub Pages
```bash
git init
git add .
git commit -m "initial: american dream sales deck"
git branch -M main
git remote add origin https://github.com/Anshul3977/american-dream-deck.git
git push -u origin main
# Then enable GitHub Pages in repo Settings → Pages → Deploy from main
```

---

## Feature Map

| Feature | Description |
|---|---|
| **Buyer Gate** | Entry screen segmenting visitors — Retail / Sponsorship / Events / Full Overview. Routes each persona to their relevant section. |
| **Non-Linear Nav** | Fixed nav + mobile hamburger. Jump to any section at any time. |
| **Retail Tabs** | 5 switchable leasing categories — Luxury, Sport, Family, F&B, Pop-Up — each with specs and CTA |
| **Competitive Table** | Side-by-side comparison vs Mall of America, West Edmonton, Hudson Yards |
| **ROI Estimator** | Interactive calculator — select investment type, budget, duration, audience → generates modeled impressions, reach, and CPM |
| **Attractions Grid** | Hover-reveal cards for all 15+ major attractions |
| **Sponsorship Tiers** | Three structured packages with pricing and feature lists |
| **World Cup 2026 Module** | Embedded urgency driver — 39-day Fan Fest, 2M visitors, FIFA adjacency |
| **Social Proof** | Awards (MAPIC Cannes, RLI London, Placer.ai #1), brand logos, milestone callouts |
| **Sticky CTA** | Persistent "Book Opportunity Review" button visible after scroll |
| **Email Capture** | CTA form with validation and confirmation state |
| **Custom Cursor** | Gold dot + ring on desktop. Disabled automatically on touch devices. |
| **Scroll Reveal** | IntersectionObserver-based staggered animations |
| **Mobile Hamburger** | Full mobile nav with smooth open/close |

---

## Design Decisions

### Why Vanilla JS (No React/Vue)?
A sales deck is a **document**, not an application. Vanilla HTML loads in under 1 second, works offline, and can be emailed as a single file. Framework overhead adds latency with zero UX benefit here.

### Why the Buyer Gate?
The #1 critique of generic sales decks: one message trying to speak to three different buyers simultaneously. A retail tenant cares about sq ft and tax arbitrage. A sponsor cares about impressions and CPM. An event planner cares about capacity and buyout pricing. The gate routes each persona to content that closes their specific deal.

### Color Palette
Deep obsidian (#080808) + brushed gold (#C9A84C) + platinum (#D4D4D4). Deliberately avoids the "shopping mall brochure" aesthetic — closer to a private equity pitch or luxury automotive brand. The gold is used sparingly — only on numbers, CTAs, and accents — to retain its visual weight.

### Copy Philosophy
Every section was written to pass the "3-second executive test" — the core metric, the argument, and the CTA must be visible before scrolling. Long paragraphs were trimmed by ~15% in the final pass. Executives skim; the deck rewards skimmers and rewards readers.

### The Estimator
Most decks show stats. This deck lets buyers model their own ROI. That shift from passive to active is the difference between a brochure and a business tool. Numbers are clearly marked as "illustrative models based on public benchmarks" to maintain credibility.

---

## AI Tools Used

| Tool | How Used |
|---|---|
| **Claude (Anthropic)** | Full deck architecture, copy writing, competitive analysis framing, all code generation, bug fixes, mobile QA, copy trimming |
| **Unsplash** | Visual assets (CDN-hosted, optimized) |
| **Google Fonts** | Typography selection and loading |

The research dossier (property facts, demographic data, sponsorship valuations, competitive benchmarks) was provided as briefing material and verified against publicly available sources before inclusion. All estimator outputs are explicitly labeled as modeled benchmarks.

---

## What I Would Improve With More Time

1. **Real video integration** — Compressed MP4 autoplay background in the hero section. Actual American Dream footage would dramatically increase emotional impact in the first 10 seconds.
2. **Calendly embed** — Replace the email capture with a direct calendar booking widget for zero-friction meeting scheduling.
3. **Persona-specific deep modules** — Separate leasing, sponsorship, and events sub-decks that open as modal overlays with deeper content specific to each buyer type.
4. **Live inquiry engine** — After the buyer gate, a short 4-question flow (brand type → sq ft → budget → timeline) that outputs a specific, personalized opportunity recommendation. This upgrades the experience from a presentation to a product.
5. **Animation polish** — The three key motion moments (Buyer Gate entrance, hero reveal, Estimator result) would benefit from GSAP-quality easing curves.
6. **Performance audit** — Lighthouse score optimization: further image compression, critical CSS inlining, font subsetting.

---

## Project Structure

```
american-dream-deck/
├── american-dream-deck.html   # Complete single-file application
├── README.md                  # This file
└── write-up.md               # Optional 1-page design rationale
```

---

## Notes on Data

All statistics sourced from publicly available data:
- Placer.ai 2023 retail footfall rankings
- NJ Division of Taxation (apparel tax)
- American Dream official press materials
- NJ Division of Travel & Tourism (2024 visitor data)
- Triple Five Group public disclosures
- FIFA World Cup 2026 official venue announcements

Estimator outputs are illustrative benchmark models, noted explicitly in the UI.

---

*Built by **Anshul Palarpwar** · [github.com/Anshul3977](https://github.com/Anshul3977)*
