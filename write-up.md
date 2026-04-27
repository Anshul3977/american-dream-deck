# Design Rationale & AI Usage Write-Up
**Project:** American Dream Meadowlands — Interactive Commercial Sales Deck  
**Candidate:** [Your Name] · [your-email@domain.com]

---

## The Core Problem I Was Solving

The brief described a sales process that is "fragmented, inconsistent, and doesn't convey scale or energy." A rep opens YouTube, flips to a PDF, reads from a spreadsheet — three tools, one story, zero cohesion. My goal was to collapse all of that into a single URL that does the selling independently.

The key insight driving every decision: **this is not a website. It is a closing tool.** That distinction shaped everything from the Buyer Gate to the Estimator to the sticky CTA.

---

## Design Decisions

### 1. The Buyer Gate (Highest-Impact Decision)
The first thing a visitor sees is a choice: Retail Leasing, Brand Sponsorship, Event Booking, or Full Overview. This is not decoration — it is the most commercially important UX decision in the project.

A retail tenant evaluating sq footage and tax arbitrage has completely different information needs than a CMO evaluating sponsorship CPM or an event planner comparing venue capacity. A deck that tries to speak to all three simultaneously speaks compellingly to none. The gate routes each persona to the content that closes their specific deal.

### 2. Data First, Story Second
Every section leads with the hardest, most credible number available — then builds the narrative around it. The hero headline is not "America's Greatest Mall." It is "Reach 40 Million Consumers Who Already Showed Up." The distinction: one is branding, one is a business proposition.

### 3. The Estimator as Product Signal
Most decks present statistics. This deck lets buyers model their own ROI by selecting investment type, budget, duration, and target audience. That shift from passive consumption to active engagement is the difference between a brochure and a business tool. It also signals product thinking — that I understand the buyer's actual decision-making process, not just the property's marketing story.

### 4. Copy Discipline
Every body paragraph was written to pass a self-imposed "3-second executive test" — the core metric, the argument, and the next action must be visible before scrolling. After the initial build, I trimmed all body copy by approximately 15%, removing every sentence that restated something already communicated visually by a stat card or headline. Executives skim. The deck rewards skimmers first, readers second.

### 5. Visual Language
Deep obsidian + brushed gold + platinum. Deliberately avoids every "shopping mall brochure" visual convention. The reference points were luxury automotive and private equity — confident, institutional, minimal. Gold was used as a precision tool, not decoration: applied only to key numbers, CTAs, and the highest-priority accents so it retains its visual weight throughout.

---

## How I Used AI

**Claude (Anthropic)** was my primary collaborator throughout the project:

- **Research synthesis:** Given the raw briefing dossier, Claude helped structure the commercial narrative — identifying which stats were strongest for each buyer persona, which objections required proactive counter-messaging, and what the competitive differentiation story should be.
- **Copy writing:** All section headlines, body copy, and CTA language were written collaboratively — with deliberate effort to strip AI-sounding phrases ("apex of the experiential economy," "devastatingly effective") in favor of precise, credible executive language.
- **Code generation:** The full HTML/CSS/JS was generated and iteratively refined — including the Buyer Gate logic, tab switching, scroll reveal, ROI estimator calculation model, mobile hamburger menu, and touch device cursor detection.
- **QA pass:** Claude performed a structured bug audit — identifying the implicit `event` global in the tab switching function (cross-browser failure risk), the missing touch device cursor override (broken UX on mobile), the estimator result visibility logic issue, and the mobile table overflow handling.

The research dossier provided the factual foundation. AI accelerated the journey from raw facts to finished product by approximately 10x — handling the translation from business intelligence to interactive experience that would otherwise require a copywriter, designer, and developer working separately.

---

## What I Would Improve With More Time

**Priority 1 — Real video in the hero.** Compressed, autoplay MP4 of actual American Dream footage. The current animated CSS background conveys scale through data; real footage conveys it through feeling. That emotional hit in the first 8 seconds is the highest-leverage improvement available.

**Priority 2 — Live inquiry engine.** After the Buyer Gate, a 4-question flow (brand category → sq ft needed → budget range → timeline) that outputs a specific, personalized opportunity — recommended zone, comparable tenant, suggested format. This upgrades the experience from a presentation to a product that actively helps the buyer make a decision.

**Priority 3 — Calendly embed.** Replace the email capture with a direct calendar widget. Zero friction between interest and scheduled conversation is worth more than any amount of copy refinement.

**Priority 4 — Persona sub-decks.** Separate leasing, sponsorship, and events modules that open as full-screen overlays with deeper, buyer-specific content — floor plans, past event case studies, detailed sponsorship activation examples.

---

*Submitted to: medi@liat.ai*  
*[Your Name] · [your-email] · [linkedin.com/in/yourhandle]*
