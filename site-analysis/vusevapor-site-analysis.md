# VuseVapor.com — Comprehensive Site Analysis

**Prepared for:** Adobe Experience Manager Migration Assessment\
**Date:** March 31, 2026\
**Analyst:** Adobe Experience Catalyst\
**Site URL:** https://www.vusevapor.com/\
**Platform:** Adobe Experience Manager (AEM) as a Cloud Service\
**Brand Owner:** R.J. Reynolds Vapor Company (Reynolds American Inc.)

---

## Executive Summary

VuseVapor.com is an age-gated vapor/e-cigarette brand website built on Adobe Experience Manager as a Cloud Service. The site requires 21+ age verification and user authentication before accessing any content. It features product showcases for two product lines (Original Series and Prismatic Series), a social content hub ("The Drop"), a rewards loyalty program ("All Access Rewards"), mobile coupons, store locator with Google Maps integration, SMS opt-in, and a blog section. The site has approximately 40+ pages across 13 identified templates and utilizes 30+ distinct UI components.

---

## 1. Templates Inventory

### Template 1: Homepage
- **URL:** `/` (root)
- **Description:** Full-featured landing page with video hero background ("Vapor Done Right"), product carousel (6 slides for Original + Prismatic series), rewards promo section, "America's #1 Vape" claim, product features list, and standard CTA trifecta (Text Sign-Up, Offers, Store Locator). Uses AEM freeform template.
- **Key Components:** Video Hero, Product Carousel, Rewards Banner, Feature List, CTA Cards Trifecta
- **Screenshot:** vuse-01-homepage.png

### Template 2: Product Landing Page (Original Series)
- **URL:** `/originals.html`
- **Description:** Product showcase with video hero, product card grid (6 products: Classic Tobacco, Golden Tobacco, Menthol + 3 All-in-One Kits), device color showcase, key features grid (SmartDraw, USA Blended, Bold Look, More Variety), and Brightcove video integration for embedded product video.
- **Key Components:** Video Hero, Product Cards Grid, Device Color Showcase, Key Features Grid, Brightcove Video Player, "Find A Store" CTA
- **Screenshot:** vuse-02-originals.png

### Template 3: Product Landing Page (Prismatic Series)
- **URL:** `/prismatic.html`
- **Description:** Similar to Originals but with Prismatic-specific products (Golden Spark Tobacco, Dusk Glow Tobacco, Aqua Frost Menthol + 2 Tasting Kits). Includes "Limited quantity remaining" disclaimer, exclusive device showcase (silver/gold), and key features grid. Different hero content and product names.
- **Key Components:** Video Hero, Product Cards Grid, Device Showcase (dual image), Key Features Grid, Promo Cards (The Drop, Rewards), CTA Cards
- **Screenshot:** vuse-05-prismatic.png

### Template 4: Products Overview
- **URL:** `/products.html`
- **Description:** Legacy products page showing older device lineup (Solo 4.8%, Vibe 3.0%, Ciro 1.5%) with comparison cards showing nicotine strength, device description, and cartridge/tank type with product imagery.
- **Key Components:** Image Hero, Product Comparison Cards (3-column), Promo Cards, CTA Cards Trifecta
- **Screenshot:** vuse-10-products.png

### Template 5: Content Hub ("The Drop")
- **URL:** `/the-drop.html`
- **Description:** Social content hub with branded header ("THE DROP"), grid of 20+ content cards including quizzes, polls, videos, and articles. Each card has Like and Comment counters showing social engagement. Content types include "Winter Games", "Real Talk", opinion polls, and interactive quizzes.
- **Key Components:** Branded Section Header, Content Card Grid (20+ cards), Like/Comment Counters, Content Type Labels (Quiz, Poll, Video)
- **Screenshot:** vuse-03-the-drop.png

### Template 6: Blog/Article Detail
- **URL:** `/blog/response-to-recent-fda-decision.html`
- **Description:** Article detail page with "The Drop" branded header, article title, publication date, featured image (branded Vuse image), article body text with bulleted lists, and Previous/Next post navigation.
- **Key Components:** Blog Header (The Drop branding), Article Title, Date, Featured Image, Article Body, Post Navigation (Previous/Next)
- **Screenshot:** vuse-13-blog-post.png

### Template 7: Mobile Coupons / Offers
- **URL:** `/mobile-coupons.html`
- **Description:** Personalized coupon page showing user-specific data ("NIHAR, You Have: 1 Coupon Available"), claimed savings tracker ($0 2026), 4-step redemption instructions with illustrations (Log In, Location Settings, Pick Offer, Redeem), and detailed coupon terms.
- **Key Components:** Hero Banner, Personalized Coupon Status, "Redeem Now" CTA, Step-by-Step Instructions (4 steps with images), Legal/Terms Disclosure, Promo Cards
- **Screenshot:** vuse-06-mobile-coupons.png

### Template 8: Store Locator
- **URL:** `/store-locator.html`
- **Description:** Full-featured store finder with hero banner, zip code search field, "Use my current location" option, product filter, store results list (10 per page with Load More), Google Maps integration with numbered markers, and store details (name, address, store ID, distance, Get Directions link).
- **Key Components:** Hero Banner, Zip Code Search Form, Product Filter, Store Results List, Google Maps Embed (Advanced Markers), Get Directions Links, Promo Cards, CTA Cards
- **Screenshot:** vuse-07-store-locator.png

### Template 9: About Us
- **URL:** `/about-us.html`
- **Description:** Rich brand story page with full-screen video hero, brand description text, interactive horizontal timeline carousel (8 slides from 2013–Today), second video section, "Distraction-Free By Design" feature callout, "Find Your Style" product selector (Original vs Prismatic), sustainability section with tabbed content (Responsible Device Disposal, Pod Recycling Program, Smarter Shipping).
- **Key Components:** Full-Screen Video Hero, Brand Description, Timeline Carousel (8 slides), Feature Video, Feature Callout, Product Style Selector (2 cards), Sustainability Tabs, Promo Cards, CTA Cards Trifecta
- **Screenshot:** vuse-08-about-us.png

### Template 10: SMS Opt-In
- **URL:** `/sms.html`
- **Description:** SMS sign-up page with hero banner, phone number input field, comprehensive legal consent checkbox (age 21+ certification, TCPA consent, recurring message agreement), Submit button (disabled until consent), and detailed T&C text.
- **Key Components:** Hero Banner, Phone Number Form, Legal Consent Checkbox, Submit CTA, Promo Cards, CTA Cards (Offers + Store Locator)
- **Screenshot:** vuse-09-sms.png

### Template 11: Rewards Enrollment
- **URL:** `/rewards-enroll.html`
- **Description:** Minimal enrollment page with "Rewards Program" heading, Terms & Conditions checkbox, and "Join All Access" button. No additional content sections. Redirects here from `/rewards/home.html` for unenrolled users.
- **Key Components:** Heading, T&C Checkbox, Join CTA
- **Screenshot:** vuse-04-rewards-enroll.png

### Template 12: How It Works (Rewards)
- **URL:** `/how-it-works.html`
- **Description:** Rewards program explainer with secondary navigation (Rewards Home, Earn, Catalog), 3-step process (Scan, Earn, Redeem) with icons, "Where's My Code?" section with pack image, "Back to Rewards" CTA, and points value table showing product-to-points mapping (1-Pod Pack +125 to 6-Pod Pack +750).
- **Key Components:** Secondary Nav (Rewards), 3-Step Process Icons, Instructional Image Section, Points Value Table, Back CTA
- **Screenshot:** vuse-12-how-it-works.png

### Template 13: FAQ / Information Pages
- **URL:** `/footer-links/faq.html`, `/footer-links/faqs.html`, `/footer-links/faqs-sustainability.html`
- **Description:** Long-form FAQ pages with categorized accordion sections. The main FAQ page covers Vuse Warnings & Information with extensive health warnings, product details, battery safety, and regulatory information. Multiple expandable sections with detailed Q&A content.
- **Key Components:** Page Title, Accordion Sections, Q&A Content, Legal Disclaimers
- **Screenshot:** vuse-11-faq.png

---

## 2. Blocks / Components Catalog

### Global Components (Present on Most Pages)

| # | Component | Description |
|---|-----------|-------------|
| 1 | **Regulatory Warning Bar** | Fixed top bar: "WARNING: This product contains nicotine. Nicotine is an addictive chemical." — Different from tobacco sites |
| 2 | **Age Gate / Underage Bar** | "VAPOR PRODUCTS / UNDERAGE SALE PROHIBITED" header strip |
| 3 | **Pack Code Reminder Bar** | Dismissible banner: "Did you enter your pack code today?" with link to rewards |
| 4 | **Main Navigation (Header)** | Vuse logo, hamburger menu, Join Rewards CTA, notification bell (with badge count), responsive mobile-first |
| 5 | **Notification Center** | Flyout panel with Available Coupons count and notification links |
| 6 | **Footer (5-Column)** | Structured footer: Legal, Terms, FAQ, Products, Get In Touch (with phone number and hours) |
| 7 | **Copyright Bar** | "©2026 R.J. Reynolds Vapor Company" |

### Content Components

| # | Component | Description | Pages Found |
|---|-----------|-------------|-------------|
| 8 | **Video Hero** | Full-width background video with overlay text and CTA button | Homepage, Originals, Prismatic, About Us |
| 9 | **Image Hero** | Static image hero with overlay heading and description | Products, Mobile Coupons, Store Locator, SMS |
| 10 | **Product Card Grid** | Grid of product cards with image, name, description, and flavor details | Originals, Prismatic |
| 11 | **Product Comparison Cards** | Side-by-side product comparison with nicotine %, description, and cartridge type | Products |
| 12 | **Product Carousel** | Horizontal scrollable carousel of product images (6 slides) with navigation dots | Homepage |
| 13 | **Timeline Carousel** | Horizontal timeline with year milestones (2013–Today) with descriptions and pagination | About Us |
| 14 | **Key Features Grid** | 2×2 or 4-column grid of feature icons with heading and description | Originals, Prismatic |
| 15 | **Device Color Showcase** | Side-by-side device images showing available color options | Originals, Prismatic |
| 16 | **CTA Cards Trifecta** | 3-card row with icon, heading, description, and link (Text Sign-Up, Offers, Store Locator) | Most pages |
| 17 | **CTA Cards Duo** | 2-card variant of CTA cards (Offers + Store Locator only) | SMS |
| 18 | **Promo Card (The Drop)** | Dark background card with "THE DROP" logo, description, and "Explore More" CTA | Most pages |
| 19 | **Promo Card (Rewards)** | Gold/tan background card with "ALL ACCESS REWARDS" logo, phone image, and "Get Rewarded" CTA | Most pages |
| 20 | **Content Card Grid** | Grid of social content cards with thumbnails, titles, Like/Comment counters | The Drop |
| 21 | **Blog Article Layout** | Article with branded header, title, date, featured image, body text, and post navigation | Blog detail pages |
| 22 | **Coupon Status Widget** | Personalized widget showing available coupons, "Redeem Now" CTA, and claimed savings | Mobile Coupons |
| 23 | **Step-by-Step Instructions** | Numbered steps (1-4) with illustrations and descriptive text | Mobile Coupons |
| 24 | **Store Search Form** | Zip code input with "Use my current location" button and product filter | Store Locator |
| 25 | **Store Results List** | Numbered list of stores with name, address, ID, distance, and Get Directions link | Store Locator |
| 26 | **Google Maps Embed** | Interactive Google Maps with numbered markers, map/satellite toggle, and fullscreen | Store Locator |
| 27 | **SMS Opt-In Form** | Phone number input with TCPA consent checkbox and Submit button | SMS |
| 28 | **Rewards Enrollment Form** | T&C checkbox with "Join All Access" CTA button | Rewards Enroll |
| 29 | **Rewards Secondary Nav** | Sub-navigation bar (Rewards Home, Earn, Catalog) | How It Works, Rewards pages |
| 30 | **3-Step Process** | Three icon-based steps with heading and description (Scan, Earn, Redeem) | How It Works |
| 31 | **Points Value Table** | Product-to-points mapping table with product names and point values | How It Works |
| 32 | **Accordion / FAQ** | Expandable Q&A sections with category headers | FAQ pages |
| 33 | **Sustainability Tabs** | Tabbed content with 3 tabs (Device Disposal, Pod Recycling, Smarter Shipping) | About Us |
| 34 | **Find Your Style Selector** | Two large cards linking to Original and Prismatic product pages | About Us, Homepage |
| 35 | **Feature Callout** | Single feature with heading and description on dark background | About Us |
| 36 | **Legal Disclosure Block** | Expandable legal terms text for coupon/offer pages | Mobile Coupons |
| 37 | **"Find A Store" CTA Button** | Standalone button linking to store locator | Originals, Prismatic, Homepage |
| 38 | **America's #1 Vape Section** | Large heading with footnote/disclaimer text | Homepage |
| 39 | **Rewards Banner** | Full-width banner with rewards messaging and CTA | Homepage |
| 40 | **DoubleClick Tracking Iframe** | Hidden iframe for Floodlight conversion tracking | All pages |

---

## 3. Page Counts by Template

| Template | Estimated Page Count | Notes |
|----------|---------------------|-------|
| Homepage | 1 | Single landing page |
| Product Landing (Originals) | 1 | Original Series products |
| Product Landing (Prismatic) | 1 | Prismatic Series products |
| Products Overview | 1 | Legacy devices (Solo, Vibe, Ciro) |
| Content Hub (The Drop) | 1 | Social content listing |
| Blog/Article Detail | 20+ | Individual articles from The Drop (quizzes, polls, videos, FDA updates) |
| Mobile Coupons | 1 | Coupon redemption page |
| Store Locator | 1 | Google Maps-powered store finder |
| About Us | 1 | Brand story with timeline |
| SMS Opt-In | 1 | Text message sign-up |
| Rewards Enrollment | 1 | Loyalty program enrollment |
| How It Works (Rewards) | 1 | Rewards program explainer |
| Rewards Sub-Pages | 4 | Home, Earn, Catalog, History (behind enrollment) |
| FAQ Pages | 3 | Warnings & Info, General FAQs, Sustainability FAQs |
| Footer/Legal Pages | 7+ | Patents, Privacy Policy, Terms of Use, Text Messaging T&C, Site Requirements, Rewards T&C, Contact Us |
| Profile/Auth Pages | 3+ | Login, Secure page, My Profile (MFA-protected) |
| 404 Error Page | 1 | Custom "gone up in vapor" error page |
| **TOTAL** | **~48–55** | |

---

## 4. Integrations Analysis

### 4.1 Adobe Experience Cloud Stack

| Integration | Details |
|-------------|---------|
| **Adobe Experience Platform Launch** | Property: `b57d62cd96da/d9b47302c1aa` — `launch-47a069065861.min.js` — 30+ extensions loaded |
| **Adobe Analytics (AppMeasurement)** | v2.27.0 — Report Suite: `raiservices.global.prod` — Org: `02D9C50759DEA0920A495ED3@AdobeOrg` |
| **Adobe Analytics Activity Map** | Module loaded for click-tracking heatmaps |
| **Adobe Audience Manager** | AppMeasurement_Module_AudienceManagement — AAM ID sync via `dpm.demdex.net` |
| **Adobe Target** | AT.js active — "View triggered on page load: secure" — Used for personalization |
| **Adobe Client Data Layer** | v2.0.2 — 59 events on homepage — Powers component-level analytics |
| **AEM Core Components Data Layer** | `core.wcm.components.commons.datalayer.v1` — Structured component tracking |

### 4.2 Third-Party Advertising & Tracking

| Integration | Details |
|-------------|---------|
| **Google DoubleClick (Floodlight)** | Conversion tracking via iframe — `8311824.fls.doubleclick.net` — Category: `allpa0` |
| **MediaIQ Digital** | `pixel.mediaiqdigital.com` — Digital media attribution |
| **MediaIQ (Honest Click)** | `honestclick.miqdigital.com` — Click fraud detection |
| **Vindico Suite** | `mpp.vindicosuite.com` — Video advertising measurement |
| **Tribal Fusion** | `s.tribalfusion.com` — Programmatic advertising |
| **AppNexus (Xandr)** | `ib.adnxs.com` — Programmatic ad exchange |
| **OpenX** | `us-u.openx.net` — Programmatic ad exchange |
| **PubMatic** | `image2.pubmatic.com` — Programmatic SSP |
| **Casale Media (Index Exchange)** | `dsum-sec.casalemedia.com` — Ad exchange |
| **Tremor Hub** | `partners.tremorhub.com` — Video ad exchange |
| **Agkn (Neustar)** | `aa.agkn.com` — Digital ad scoring |
| **Rezync** | `live.rezync.com` — Ad sync/retargeting |
| **Everest Tech (Adobe Ad Cloud)** | `sync-tm.everesttech.net` — Adobe Advertising Cloud sync |
| **RLCDn (LiveRamp)** | `idsync.rlcdn.com` — Identity resolution |
| **Google Ads** | `cm.g.doubleclick.net` — Cookie matching for Google Ads |
| **BrightTag (Signal)** | `s.thebrighttag.com` — Tag management/data onboarding |
| **Stickyadstv** | `ads.stickyadstv.com` — Video advertising (410 Gone — deprecated) |

### 4.3 Platform & Application Integrations

| Integration | Details |
|-------------|---------|
| **Brand Site API** | `https://api.vusevapor.com` — Site key: `vuse` — Authentication, profile, coupons, store data |
| **Loyalty Plus** | `clientlib-vuse` — Rewards program engine — Points, catalog, redemption |
| **Google Maps API** | Advanced Markers, Map/Satellite, Fullscreen, Street View — Store locator |
| **Google Fonts** | Roboto (400/500/700) via `fonts.googleapis.com` |
| **MyFonts** | Custom font loading via `hello.myfonts.net/count/3be03d` |
| **RUM (Real User Monitoring)** | `rum.hlx.page` — Adobe Helix RUM standalone v2 |
| **Service Worker** | `resource-cache-service-worker.js` with `vuse-cache-config.json` — Resource caching |
| **Google Site Verification** | `yqCmh0AA-jPuWWDvzRl7IN6qhLMAYY1umVi3_6yCVsU` |

### 4.4 Client Libraries (AEM)

| Library | Purpose |
|---------|---------|
| `reynoldsamerican-aem-base/clientlib-dependencies` | Shared RAI base CSS/JS |
| `vuse/clientlib-dependencies` | Vuse-specific dependencies |
| `vuse/clientlib-all` | Vuse site-wide CSS/JS |
| `loyaltyplus/clientlib-vuse` | Loyalty Plus rewards integration |
| `core/wcm/components/commons/datalayer/v1` | AEM Core Components data layer |

**Total Integrations Identified: 32+**

---

## 5. Complex Use Cases & Observations

### 5.1 Age-Gated Authentication System
- Multi-step age verification and authentication flow
- Cross-brand SSO via RAI services (shared with camel.com, americanspirit.com, camelsnus.com)
- `securePage()` function controls page access with API endpoint and site key
- Service worker for resource caching (`resource-cache-service-worker.js`)
- Secure page pattern redirects unauthenticated users to `/login`
- Profile pages use Multi-Factor Authentication (MFA) — profile URL returns 404 without proper MFA session

### 5.2 Vapor-Specific Regulatory Requirements
- **Different warning**: "WARNING: This product contains nicotine. Nicotine is an addictive chemical." (vs. tobacco warnings on other RAI sites)
- **Different header**: "VAPOR PRODUCTS / UNDERAGE SALE PROHIBITED" (unique to vapor category)
- FDA Marketing Granted Order references (Vuse Solo, 2021)
- PMTA (Premarket Tobacco Product Application) status updates in blog content
- Emergency stay of enforcement legal updates

### 5.3 Rewards Program ("All Access Rewards")
- Loyalty Plus platform integration with Vuse-specific client library
- Pack code scanning (physical product to digital points)
- Monthly point limits: 3,750 points per month
- Point values range from +125 (1-Pod Pack) to +750 (6-Pod Pack)
- Rewards catalog with digital gift cards, coupons, and more
- Separate enrollment flow with T&C acceptance
- Non-enrolled users redirected from `/rewards/home.html` to `/rewards-enroll.html`

### 5.4 Mobile Coupon System
- Personalized coupon display (user-specific coupon count and savings)
- Location-based redemption requiring mobile device and GPS
- 5-minute redemption timer for in-store use
- Coupon tracking with claimed savings calculation
- Calendar year savings reset
- Notification center integration (coupon badge count)

### 5.5 Content Hub ("The Drop")
- Social content platform with engagement metrics (Likes, Comments)
- Multiple content types: quizzes, polls, videos, articles
- Content cards with visual thumbnails and engagement counters
- Blog detail pages with "The Drop" branded header
- Post navigation (Previous/Next)
- Potentially dynamic/API-driven content loading

### 5.6 Dual Product Line Architecture
- Two distinct product lines with separate pages: Original Series and Prismatic Series
- Prismatic Series has "Limited quantity remaining" disclaimer
- Legacy products (Solo, Vibe, Ciro) on separate Products page
- Product carousel on homepage combines both lines
- Store locator has "Filter by Product" capability

### 5.7 Extensive Ad Tech Stack
- 17+ third-party advertising/tracking integrations
- Video advertising (Vindico Suite, Stickyadstv)
- Programmatic ad exchanges (AppNexus, OpenX, PubMatic, Index Exchange)
- Identity resolution (LiveRamp, Neustar)
- Adobe Advertising Cloud sync (Everest Tech)
- Some integrations returning errors (410 Gone for Stickyadstv — likely deprecated)

### 5.8 Sustainability Section
- Tabbed content section (3 tabs: Responsible Device Disposal, Pod Recycling Program, Smarter Shipping)
- Partnership with The Battery Network (formerly Call2Recycle)
- "Find Recycling Locations" CTA
- ~70% device weight recycling claim
- Limited geographic availability disclaimer

### 5.9 Google Maps Integration
- Advanced Markers API (gmp-advanced-marker)
- Numbered store markers
- Map/Satellite view toggle
- Fullscreen mode
- Street View Pegman
- Distance calculation from search location
- "Get Directions" links opening Google Maps

### 5.10 Custom 404 Page
- Branded error page: "Sorry, that page has gone up in vapor"
- "GO BACK" CTA button
- Vapor-themed messaging consistent with brand identity

---

## 6. Migration Estimates

### 6.1 Effort Breakdown

| Work Stream | Estimated Person-Days | Complexity |
|-------------|----------------------|------------|
| **Design System Migration** | 15–20 | Medium-High |
| — Global CSS tokens, typography (Roboto + custom MyFonts) | | |
| — Responsive breakpoints, grid systems | | |
| — Dark/gold/navy color themes | | |
| **Global Components** | 20–25 | High |
| — Regulatory warning bars (vapor-specific) | | |
| — Age gate / underage bar | | |
| — Pack code reminder bar | | |
| — Header with notification center | | |
| — Footer (5-column with contact info) | | |
| **Content Blocks (Standard)** | 25–30 | Medium |
| — Video Hero with overlay | | |
| — Image Hero | | |
| — Product Card Grids | | |
| — Key Features Grid | | |
| — CTA Cards (Trifecta/Duo) | | |
| — Promo Cards (The Drop/Rewards) | | |
| — FAQ Accordion | | |
| — Step-by-Step Instructions | | |
| **Content Blocks (Complex)** | 30–40 | High |
| — Product Carousel (6-slide) | | |
| — Timeline Carousel (8-slide with pagination) | | |
| — Content Hub Card Grid (with engagement metrics) | | |
| — Sustainability Tabs (3-tab interface) | | |
| — Store Locator (Google Maps + results list) | | |
| — Blog Article Layout (with post navigation) | | |
| **Interactive Features** | 35–45 | Very High |
| — Mobile Coupon System (personalized, location-based) | | |
| — Rewards Integration (Loyalty Plus) | | |
| — SMS Opt-In Form (TCPA compliance) | | |
| — Notification Center | | |
| — Pack Code Entry | | |
| — Product Filter (Store Locator) | | |
| **Authentication & Security** | 20–25 | Very High |
| — SSO/VIA integration | | |
| — MFA for profile pages | | |
| — Age verification flow | | |
| — Service worker migration | | |
| **Content Migration** | 15–20 | Medium |
| — ~48–55 pages across 13 templates | | |
| — 20+ blog/article pages | | |
| — FAQ content (extensive) | | |
| — Legal/terms pages | | |
| **Analytics & Tracking** | 15–20 | High |
| — Adobe Analytics with 30+ Launch extensions | | |
| — Adobe Target personalization | | |
| — 17+ ad tech integrations | | |
| — Conversion tracking (DoubleClick Floodlight) | | |
| — Client Data Layer migration | | |
| **Testing & QA** | 20–25 | High |
| — Cross-browser/device testing | | |
| — Age gate flow testing | | |
| — Coupon redemption testing | | |
| — Store locator accuracy | | |
| — Accessibility (WCAG 2.1 AA) | | |
| — Performance optimization | | |

### 6.2 Summary Estimates

| Scenario | Total Person-Days | Calendar Duration |
|----------|-------------------|-------------------|
| **Optimistic** (experienced team, parallel tracks) | 195 | 10–12 weeks |
| **Realistic** (standard team, some dependencies) | 250 | 14–16 weeks |
| **Conservative** (complex integrations, regulatory review) | 310 | 18–22 weeks |

### 6.3 Risk Factors

| Risk | Impact | Mitigation |
|------|--------|------------|
| **Vapor-specific regulatory compliance** | High | Legal review of all health warnings and disclaimer text |
| **Loyalty Plus integration complexity** | High | Early API contract definition with rewards team |
| **Mobile coupon location services** | Medium | Progressive enhancement for location-denied users |
| **17+ ad tech integrations** | Medium | Phased migration with analytics parity testing |
| **Cross-brand SSO dependencies** | High | Coordinate with RAI authentication team |
| **Google Maps API migration** | Medium | Verify API key and billing for new domain |
| **Content hub engagement metrics** | Medium | Define data source for likes/comments in EDS |
| **FDA/regulatory content updates** | Low-Medium | Establish rapid content update workflow |

### 6.4 Recommended Migration Phases

**Phase 1 (Weeks 1–6): Foundation**
- Design system, global components, authentication framework
- Static pages (About Us, FAQ, legal/terms pages)

**Phase 2 (Weeks 7–12): Product & Content**
- Product landing pages (Originals, Prismatic, Products)
- Blog/article template and content migration
- Content hub (The Drop) with engagement metrics

**Phase 3 (Weeks 13–18): Interactive Features**
- Store locator with Google Maps
- Mobile coupons system
- SMS opt-in
- Rewards integration (Loyalty Plus)

**Phase 4 (Weeks 19–22): Integration & Launch**
- Full analytics/ad tech stack migration
- Performance optimization
- UAT testing and regulatory compliance review
- Phased go-live with monitoring

---

## Appendix: Screenshots Reference

| Screenshot | Page | Description |
|-----------|------|-------------|
| vuse-01-homepage.png | Homepage | Video hero, product carousel, rewards section |
| vuse-02-originals.png | Originals | Product cards, device colors, key features |
| vuse-03-the-drop.png | The Drop | Content hub with social engagement cards |
| vuse-04-rewards-enroll.png | Rewards Enroll | T&C acceptance and Join CTA |
| vuse-05-prismatic.png | Prismatic | Prismatic products, exclusive device showcase |
| vuse-06-mobile-coupons.png | Mobile Coupons | Personalized coupons, redemption instructions |
| vuse-07-store-locator.png | Store Locator | Google Maps, store search, results list |
| vuse-08-about-us.png | About Us | Timeline, sustainability tabs, brand story |
| vuse-09-sms.png | SMS | Text sign-up form with TCPA consent |
| vuse-10-products.png | Products | Legacy devices (Solo, Vibe, Ciro) |
| vuse-11-faq.png | FAQ | Accordion-style warnings and information |
| vuse-12-how-it-works.png | How It Works | Rewards process and points value table |
| vuse-13-blog-post.png | Blog Post | FDA decision article with post navigation |
