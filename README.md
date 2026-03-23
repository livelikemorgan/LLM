LiveLikeMorgan — Landing Page
Brand: LLM (a division of The Mia Cimone Experience)  
Rep: LLM 
Live Booking Link: calendly.com/morgannyameye/strategy-call
---
Overview
This is a single-page HTML landing page for LLM's social media and events services. It is built with plain HTML, CSS, and vanilla JavaScript — no frameworks, no build tools, no dependencies. The entire site lives in one file and can be opened directly in any browser or deployed to any static hosting platform.
The page is designed to convert visitors into booked strategy calls by leading them through a problem-aware narrative: pain points → solution → packages → call to action.
---
Brand & Mission
LLM helps businesses and event organizers grow their brand and fill their events using proven organic social media strategies — no ad spend required.
LLM brings 7 years of experience and a track record of 1M+ organic views to every client engagement. The mission is to deliver real, measurable results through structured content strategy, consistent posting, and smart event promotion — so clients see sustainable growth without draining their budgets on paid ads.
---
Services Offered
Service	Description
Social Media Management	Full management of client Instagram, Facebook, and other platforms — strategy, scheduling, and engagement
Content Creation	Original graphics, captions, and branded post materials tailored to each client's audience
Video Editing	Reels, Stories, and feed video content edited for maximum engagement
Social Media Marketing	Hashtag research, audience growth tactics, and organic reach strategies
Event Promotion	Pre, during, and post-event organic promotion campaigns across multiple platforms
Event Planning	Full-service event coordination — concept, vendor management, on-site support, and post-event recap
---
Page Structure
The landing page is broken into the following sections in order:
Header — Logo (`LiveLikeMorgan`) + "Book Your Strategy Call" CTA button linking to Calendly
Hero — Main headline, subheading, dual CTA buttons, and a results card showing key stats (1M+ views, 7 years experience, $0 ad spend)
Problems Section — Four pain point cards targeting the core audience struggles (ad spend, inconsistent posting, empty events, no time)
Solution Section — Three-step organic growth system explanation
Packages Section — Three pricing tiers (Starter, Growth, Premium)
CTA Banner — Final conversion push linking to Calendly
Footer — Copyright line
---
Packages
Package	Price	Best For
Starter	$650/month	Businesses establishing a consistent social presence
Growth ⭐ Most Popular	$800–$1,200/month	Social media management + event promotion
Premium	$1,500–$2,500/event	Full-service event planning and promotion
---
Tech Stack
Layer	Details
Markup	HTML5
Styling	CSS3 — custom properties, animations, grid, flexbox
Scripting	Vanilla JavaScript (scroll reveal, smooth anchor scroll)
Fonts	Google Fonts — `Fraunces` (display/headings), `Outfit` (body)
Dependencies	None — fully self-contained except Google Fonts CDN
Framework	None
Build Tool	None
---
Color Palette
Variable	Hex	Usage
`--fire-orange`	`#FF6B35`	Primary CTA, highlights, accents
`--sun-gold`	`#FFB627`	Underline accents, gradients
`--river-teal`	`#00838F`	Badge, checkmarks, secondary accents
`--warm-cream`	`#FFF8E7`	Page background
`--charcoal`	`#1A1A1A`	Body text, dark sections
`--coral-pink`	`#FF8C69`	Gradient blends
`--soft-white`	`#FEFEFE`	Card backgrounds
---
Typography
Font	Role	Weights Used
Fraunces (serif)	Headings, stat numbers, logo	400, 700, 900 italic
Outfit (sans-serif)	Body copy, buttons, labels	400, 500, 600, 700, 800
---
Animations & Interactions
Background blobs — three SVG-free CSS blobs that morph and float continuously using `@keyframes morphBlob`
Hero entrance — `slideDown` (header) and `fadeInUp` / `fadeInRight` (hero content) on page load
Highlight underline — the italic headline word animates a gold underline on load via `@keyframes underlineGrow`
Badge glow — the teal badge pulses with a glow animation
Scroll reveal — `.scroll-reveal` elements fade up into view using `IntersectionObserver`
Card hover effects — lift + shadow on all cards via CSS transitions
Results card tilt — the hero card is rotated `-2deg` and snaps flat on hover
CTA ripple — button hover triggers an expanding circle overlay using `::before` pseudo-element
---
Developer Notes
Updating Content
All text content is inline in the HTML — no CMS or templating. To update:
Headline / subheading → find `<h1>` and `<p class="subheading">` in the `<section class="hero">` block
Stats → update `.stat-number` and `.stat-label` values in the `.results-card` div
Package prices or features → find `<section class="packages-section">` and edit `.package-price` and `.package-features li` elements
Calendly link → search for `calendly.com/morgannyameye/strategy-call` — appears in the header CTA and the final CTA banner
Updating the Logo / Brand Name
The logo text `LiveLikeMorgan` is in the `<header>` inside `<div class="logo">`. Update it there and in the `<title>` tag in `<head>`.
Adding a New Section
Add a new `<section>` block between existing ones. Use `class="scroll-reveal"` on inner containers to get the scroll animation automatically. Follow the existing color pattern — alternate between `background: white`, `background: var(--charcoal)`, and `background: var(--warm-cream)`.
Deployment
Since this is a single HTML file with no build step:
Drag and drop onto any static host (Netlify, Vercel, GitHub Pages, Hostinger, GoDaddy)
Or upload directly via FTP/cPanel file manager
Google Fonts loads from CDN — an internet connection is required for fonts to render correctly
Footer Copyright Year
The footer currently reads `© 2019 Morgan Social`. Update to the current year and confirm the brand name (`Morgan Social` vs `LLM` / `The Cimone Experience`) before going live.
---
Contact & Booking
All CTAs on the page point to the Calendly strategy call link:  
https://calendly.com/morgannyameye/strategy-call
To change the booking destination, do a find-and-replace on the URL across the file.
