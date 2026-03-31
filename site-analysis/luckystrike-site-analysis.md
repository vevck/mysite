# LuckyStrike.com - Comprehensive Site Analysis

**Prepared for:** Adobe Edge Delivery Services Migration Assessment
**Date:** March 31, 2026
**Analyst:** Adobe Experience Catalyst
**URL:** https://www.luckystrike.com/
**Brand Owner:** R.J. Reynolds Tobacco Company (subsidiary of Reynolds American Inc. / BAT)
**Product Category:** Cigarettes

---

## Executive Summary

LuckyStrike.com is a premium consumer-facing brand website for Lucky Strike cigarettes, operated by R.J. Reynolds Tobacco Company under the RAI Services umbrella. The site is built on **Adobe Experience Manager (AEM) as a Cloud Service** and shares the same RAI platform architecture as other Reynolds American brand sites (americanspirit.com, camel.com, camelsnus.com, vusevapor.com, cougardips.com).

Lucky Strike positions itself as "An American Original" with a bold, music-themed brand identity. The site is notably **feature-rich** compared to other RAI brand sites, with a loyalty/rewards program ("Luckies Rewards"), a substantial content hub ("American Originals"), interactive sweepstakes, Brightcove video integration, and extensive promotional features.

**Key Characteristics:**
- Age-gated (21+) with VIA/SSO cross-brand authentication
- MFA-protected profile management
- Health warning: "SURGEON GENERAL'S WARNING: Smoking By Pregnant Women May Result in Fetal Injury, Premature Birth, And Low Birth Weight."
- Product label: "CIGARETTES"
- Loyalty/rewards program ("Luckies Rewards") with QR code scanning, points, and redemption
- Content hub ("American Originals") with articles, videos, quizzes, and interactive content
- Interactive sweepstakes ("Luckies' Garage") with gamification
- Brightcove video player integration throughout
- Personalized mobile coupons with in-store redemption
- Notification bell system with available offers count
- SMS text alerts signup
- Brand history timeline with juxtapose slider and interactive poll
- Salesforce live chat support on Contact Us page

---

## 1. Templates Inventory

### Template 1: Age Gate / Login Page
**URL:** `https://www.luckystrike.com/`
**Complexity:** High
**Reasoning:** VIA/SSO cross-brand authentication with email/password login, Remember Me, registration flow with email pre-check, forgot username/password flows. Integrates with shared RAI identity system.

**Layout Structure:**
- Lucky Strike logo (red circle emblem)
- Hero image with "AN AMERICAN ORIGINAL" heading and welcome text
- Sign In form (email, Remember Me checkbox, password, LOGIN button)
- Forgot Username / Password links
- Separator
- Register section with benefits list and email input + "Join Now" button
- Age verification legal text
- Footer with legal links and Surgeon General's warning

### Template 2: Homepage (Authenticated)
**URL:** `https://www.luckystrike.com/secure.html`
**Complexity:** High
**Reasoning:** Multi-section homepage with personalized greeting, video hero, rewards CTA, Brightcove video, promotional banner, carousel, dual CTA cards, and notification system. Heavy JavaScript interactivity.

**Layout Structure:**
- Header with logo, hamburger menu, "Join Rewards" button, notification bell with count
- Federal court notice banner (scrollable)
- Personalized welcome banner ("WELCOME BACK, NIHAR")
- "Originals Get Rewarded" section with image and CTA
- Brightcove video background section
- Brand statement section with "Stay Original" messaging
- Sweepstakes promotion ("Luckies' Garage") with image, details, and "Enter Now" CTA
- Dual-card section: "Get Rewarded" (coupons) + "Luckies Lounge Live Now" (rewards dashboard)
- Content carousel (3 slides) with article cards from American Originals
- Dual CTA section: "Get Exclusive Updates" (SMS signup) + "Find Your Luckies" (store locator)
- Footer with navigation, social links, and Surgeon General's warning

### Template 3: Products Listing
**URL:** `https://www.luckystrike.com/secure/products.html`
**Complexity:** High
**Reasoning:** Video background hero, product carousel with 6 products, each with name/description/availability info. Interactive carousel with labeled pagination dots. Additional CTAs for history and content hub.

**Products (6):**
1. Red Filters - Bold flavor, Kings & 100s
2. Gold Filters - Smooth taste, Kings & 100s
3. Menthol - Refreshing, Kings & 100s
4. Menthol Silver - Subtly smooth, Kings & 100s
5. Activate Blue - Customizable menthol with capsule, Kings only
6. Activate Green - Extra menthol surge with capsule, Kings only

### Template 4: Product Detail (Category)
**URL:** `https://www.luckystrike.com/secure/products/non-menthol.html`
**Complexity:** Medium
**Reasoning:** Alternating product sections with video backgrounds and product descriptions. Two products per page (Gold Filters, Red Filters for non-menthol). Store locator CTA at bottom.

**Layout Structure:**
- Video background hero with product tagline
- Product 1: Image + name + description + availability
- Video background transition
- Product 2: Image + name + description + availability
- Store locator CTA banner

### Template 5: American Originals (Content Hub)
**URL:** `https://www.luckystrike.com/secure/luckies-american-originals.html`
**Complexity:** High
**Reasoning:** Massive content hub page with 25+ article cards, Brightcove video embeds, category filtering, and various content types (articles, videos, quizzes, interactive features). Functions as an editorial magazine within the brand site.

**Content Types:**
- Long-form articles with hero images
- Video content (Brightcove player)
- Interactive quizzes ("Can You Name That Instrument?")
- Photo essays
- Music/culture-themed content aligned with brand identity

### Template 6: Sweepstakes / Promotion (Interactive Game)
**URL:** `https://www.luckystrike.com/secure/promotions/luckies-garage.html`
**Complexity:** High
**Reasoning:** "Luckies' Garage" interactive band/music-themed game with instant win mechanics ($100 daily, $2,000 weekly, $10,000 grand prize). Includes animated hero, game start button, prize display, legal disclaimers, and links to Official Rules and FAQs.

**Prize Structure:**
- 300+ winners
- $100 daily prizes
- $2,000 weekly prize
- $10,000 grand prize
- Running 2/19/26 - 4/30/26

### Template 7: Brand History / About Us
**URL:** `https://www.luckystrike.com/secure/history.html`
**Complexity:** High
**Reasoning:** Interactive timeline spanning 1871-2020s with juxtapose (before/after) slider, 7 era sections each with image carousels, historical narrative text, and an interactive poll. Knight Lab Juxtapose integration.

**Timeline Eras:**
1. 1871 - Born in America
2. 1900s - Striking it Lucky
3. 1930s - A Legacy of Fine Tobacco
4. 1940s - A New Look for Luckies
5. 1960s - Filters, Flavor, and Fresh Beginnings
6. 1990s - Icons Never Go Out of Style
7. 2020s - Always an American Original

**Interactive Features:**
- Juxtapose before/after image slider (Knight Lab)
- Image carousels per era with prev/next navigation
- Interactive poll: "Which decade had your favorite Lucky Strike pack design?" (1930s, 1960s, 2020s)

### Template 8: Store Locator
**URL:** `https://www.luckystrike.com/secure/store-locator.html`
**Complexity:** Medium-High
**Reasoning:** Google Maps with zip code search, geolocation, store results with distance, "Products Available" expandable accordion per store, and "Get Directions" links.

### Template 9: Coupons
**URL:** `https://www.luckystrike.com/secure/coupons.html`
**Complexity:** High
**Reasoning:** Personalized coupon display with user greeting, offer count, "View Coupon" button, year-to-date savings tracker, 4-step redemption instructions, legal terms, and store locator CTA.

### Template 10: SMS Signup
**URL:** `https://www.luckystrike.com/secure/sms.html`
**Complexity:** Medium
**Reasoning:** SMS opt-in form with phone number input, legal consent checkbox, and submit button. Hero image with "$1.50 Mobile Coupon" promotional graphic.

### Template 11: Rewards Enrollment
**URL:** `https://www.luckystrike.com/secure/rewards-enroll.html`
**Complexity:** Medium
**Reasoning:** Rewards program enrollment with hero image, terms acceptance checkbox, "START EARNING" button, and link to How It Works page. Part of the Loyalty Plus system.

### Template 12: How It Works (Rewards)
**URL:** `https://www.luckystrike.com/secure/how-it-works.html`
**Complexity:** Medium
**Reasoning:** 5-step visual guide for the rewards program with video, step-by-step instructions with device mockup images, and "Rewards Home" CTA.

**Steps:**
1. Scan the QR Code
2. Find Your Code
3. Enter Your Code
4. Rack Up Points
5. Redeem Points

### Template 13: Contact Us
**URL:** `https://www.luckystrike.com/secure/footer-links/contact-us.html`
**Complexity:** Medium
**Reasoning:** Multi-channel contact page with Chat (Salesforce), Email form (topic dropdown with 9 categories + message), and Call button (1-888-566-5952). Operating hours displayed.

### Template 14: FAQ
**URL:** `https://www.luckystrike.com/secure/footer-links/faq.html`
**Complexity:** Medium
**Reasoning:** Accordion-based FAQ with 6 categories, anchor-linked table of contents, and "Need Further Assistance?" section. Categories: Offers & Promotions, Age Verification, Privacy, Troubleshooting, Product Quality, Environmental Stewardship.

### Template 15: Legal / Policy Pages
**URLs:**
- `https://www.luckystrike.com/secure/footer-links/terms-of-use.html`
- `https://www.luckystrike.com/secure/footer-links/privacy-policy.html`
- `https://www.luckystrike.com/secure/footer-links/site-requirements.html`
- `https://www.luckystrike.com/secure/footer-links/textmessaging.html`
- `https://www.luckystrike.com/secure/footer-links/rewards-terms-and-conditions.html`
**Complexity:** Low
**Reasoning:** Standard long-form legal text with anchor links and section headings. Template is reused across 5+ pages.

### Template 16: My Profile (MFA-Protected)
**URL:** `https://www.luckystrike.com/secure/my-profile.html`
**Complexity:** High
**Reasoning:** MFA-protected profile management. Passcode sent to email, verification overlay. Full profile form behind MFA gate with state selection dropdown and personal information management.

### Template 17: Article / Content Page
**URLs:** Various under `/secure/luckies-american-originals/`
**Complexity:** Medium
**Reasoning:** Individual article pages from the American Originals content hub. Includes hero image/video, article body text, related content links. Multiple content formats (text, video, quiz, interactive).

### Template 18: Promotion FAQs
**URL:** `https://www.luckystrike.com/secure/promotions/luckies-garage/faqs.html`
**Complexity:** Low
**Reasoning:** Promotion-specific FAQ page with Q&A format. Linked from sweepstakes pages.

---

## 2. Blocks / Components Catalog

### Navigation & Chrome Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 1 | **Header with Rewards & Notifications** | Fixed header: Logo (left), hamburger menu, "Join Rewards" button, notification bell with badge count showing available offers. Notification dropdown with "Available Offers" link and "Latest Activity" list | High | All `/secure/` pages |
| 2 | **Hamburger Navigation Menu** | Slide-out menu: Products (with submenu), American Originals, Sweepstakes, About Us, Store Locator, Coupons (with count badge), My Profile. Includes full footer within menu | Medium | All pages |
| 3 | **Footer** | Two-row layout: Row 1 = Products, Store Locator, Logout; Row 2 = Contact Us, FAQ, Tobacco Rights, Site Requirements, Sustainability, Terms of Use, Privacy Policy, Text Messaging T&C, Rewards T&C. Social links icon (SMS). Surgeon General's warning with "CIGARETTES" label | Medium | All pages |
| 4 | **Surgeon General's Warning Banner** | Persistent banner: "CIGARETTES" label + Surgeon General's warning image. Present on all pages | Low | All pages |
| 5 | **Federal Court Notice Banner** | Scrollable banner at top: "A Federal Court has ordered R.J. Reynolds Tobacco..." with link to health effects statements | Low | Homepage |

### Hero & Promotional Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 6 | **Welcome Banner (Personalized)** | Full-width banner with personalized greeting "WELCOME BACK, [NAME]" | Low | Homepage |
| 7 | **Video Background Hero** | Full-width hero section with Brightcove autoplay video background, overlaid heading text. Used on products pages | High | Products, Product Detail |
| 8 | **Image Hero with CTA** | Full-width hero image with heading, description text, and action button | Medium | Homepage, Sweepstakes |
| 9 | **Sweepstakes Promotion Banner** | Rich promotional section with background image, "American Originals" branding, date range, prize details, "Enter Now" CTA, and legal disclaimer with Official Rules link | High | Homepage, Sweepstakes |
| 10 | **Prize Display Section** | Visual display of prize tiers: 300+ winners, $100 daily, $2,000 weekly, $10,000 grand prize with styled typography | Medium | Sweepstakes |
| 11 | **Brand Statement Section** | Full-width image with "STAY ORIGINAL" branding and brand manifesto text. Video/image hybrid | Medium | Homepage, Products |

### Content & Card Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 12 | **Content Carousel** | Horizontal scrolling carousel with 3+ article cards, pagination dots. Each card has background image/video, title, subtitle, and CTA button | High | Homepage |
| 13 | **Article Card (Content Hub)** | Card with hero image/video, title, description, and CTA. Used in content hub grid and carousel | Medium | American Originals, Homepage |
| 14 | **Dual CTA Card Section** | Side-by-side card layout: left card (text + CTA) and right card (text + CTA). Used for paired promotions/features | Medium | Homepage (Get Rewarded + Find Luckies) |
| 15 | **Rewards + Dashboard Card** | Split card: left side "Originals Get Rewarded" with coupon CTA, right side "View Dashboard" button for rewards | Medium | Homepage |

### Product Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 16 | **Product Carousel** | Horizontal carousel with labeled pagination dots for each product (Red Filters, Gold Filters, etc.). Each slide shows product image, name, description, and availability | High | Products |
| 17 | **Product Detail Section** | Product image with name, description text, and availability info (Kings & 100s / Kings Only). Used in alternating left/right layout | Medium | Product Detail |
| 18 | **Product Availability Badge** | Text badge showing "AVAILABLE IN KINGS & 100s" or "AVAILABLE IN KINGS ONLY" | Low | Products, Product Detail |

### Interactive / Functional Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 19 | **Google Maps Store Locator** | Map with zip code search, "Use My Location" geolocation, store results with distance, "Get Directions" link, and "Products Available" expandable per store | High | Store Locator |
| 20 | **Notification Bell System** | Bell icon in header with badge count. Dropdown shows "Available Offers" with count and "Latest Activity" feed | High | All authenticated pages |
| 21 | **Interactive Poll** | Image-based poll with radio buttons (e.g., "Which decade had your favorite pack design?" with decade options showing pack images) | Medium | History |
| 22 | **Juxtapose Before/After Slider** | Knight Lab Juxtapose widget for comparing two images with draggable slider. Used for historical before/after comparisons | Medium | History |
| 23 | **Interactive Sweepstakes Game** | Gamified sweepstakes experience ("Luckies' Garage") with animated interactions, instant win mechanics, and prize reveals | High | Sweepstakes |

### Timeline & History Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 24 | **Timeline Era Section** | Decade section with year badge, heading, descriptive text, and image carousel. 7 sections create a scrolling timeline | Medium | History |
| 25 | **Image Carousel (with Navigation)** | Previous/Next button carousel for historical images within each era section | Medium | History |

### Rewards Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 26 | **Rewards Enrollment Block** | Hero with "Originals Get Rewarded", terms acceptance checkbox, "START EARNING" button, and "How it works" link | Medium | Rewards Enroll |
| 27 | **How It Works Steps** | 5-step visual guide with numbered step badges, headings, descriptions, and device mockup images showing each step | Medium | How It Works |
| 28 | **Rewards Video Player** | Embedded video player with play button overlay and thumbnail for rewards explainer video | Medium | How It Works |
| 29 | **Savings Tracker** | "$0 Saved So Far in 2026!*" personalized savings counter on coupons page | Low | Coupons |

### Coupon Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 30 | **Personalized Coupon Display** | Personalized greeting ("Hey NIHAR"), offer status ("You've got offers!"), "View Coupon" button, and savings tracker | High | Coupons |
| 31 | **Coupon Redemption Steps** | 4-step visual instructions: Log In, Reveal, Pick, Redeem. Each with heading and description | Low | Coupons |
| 32 | **Coupon Mobile Preview Image** | Phone mockup image showing "$1.50 Mobile Coupon" with Lucky Strike packaging | Low | SMS, Coupons |

### Form & Contact Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 33 | **Contact Form (Multi-Channel)** | Chat button (Salesforce), Email form (9-category dropdown + message textarea + submit), Call button (1-888-566-5952) | Medium | Contact Us |
| 34 | **Salesforce Live Chat Widget** | Floating chat bubble "Hello, have a question? Let's chat." Salesforce-powered | High | Contact Us |
| 35 | **SMS Signup Form** | Phone number input with certification checkbox (TCPA-compliant consent text) and Sign Up button | Medium | SMS |
| 36 | **Login Form** | Email + Remember Me + Password + LOGIN button. Includes forgot username/password links | Medium | Login page |
| 37 | **Registration Pre-Check** | Email input + "Join Now" button for registration flow. Benefits list (weekly coupons, exclusive content) | Medium | Login page |

### Content & Legal Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 38 | **Accordion / FAQ Block** | Expandable Q&A sections grouped by category. Click heading to expand answer. Used across FAQ pages | Medium | FAQ |
| 39 | **Anchor Table of Contents** | In-page navigation links to FAQ categories with anchor references | Low | FAQ |
| 40 | **Long-Form Legal Content** | Structured legal text with headings, paragraphs, lists, and "Back to Top" navigation | Low | Terms, Privacy, etc. |

### Authentication Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 41 | **MFA Passcode Overlay** | Modal overlay: "Enter Passcode" with target email display, passcode input, Continue button, and help text | High | My Profile |

### Utility Components

| # | Component | Description | Complexity | Reference URL(s) |
|---|-----------|-------------|------------|-------------------|
| 42 | **Brightcove Video Player** | Embedded Brightcove player (account 6134468300001) used for product videos, content hub, and rewards explainer | Medium | Products, American Originals, How It Works |
| 43 | **Store Locator CTA Banner** | "Find A Retailer Near You / Looking For Luckies?" with Store Locator button link. Reused across pages | Low | Products, Coupons |

**Total Unique Components: 43**

---

## 3. Page Counts by Template

| Template | Est. Page Count | Migration Type | Notes |
|----------|----------------|----------------|-------|
| Age Gate / Login | 1 | Manual | Complex auth integration |
| Homepage | 1 | Manual | Heavy interactivity, personalization |
| Products Listing | 1 | Manual | Video backgrounds, carousel |
| Product Detail (Category) | 2-3 | Semi-Auto | Non-menthol, Menthol, possibly Activate |
| American Originals (Hub) | 1 | Manual | Complex content hub layout |
| Article / Content Pages | 15-25 | Semi-Auto | Individual articles, varies by content type |
| Sweepstakes / Promotion | 2-3 | Manual | Interactive game, seasonal |
| Brand History / About | 1 | Manual | Juxtapose, carousels, poll |
| Store Locator | 1 | Manual | Google Maps integration |
| Coupons | 1 | Manual | Personalized, API-driven |
| SMS Signup | 1 | Semi-Auto | Form with legal consent |
| Rewards Enrollment | 1 | Manual | Loyalty Plus integration |
| How It Works | 1 | Semi-Auto | Step-based layout with images |
| Contact Us | 1 | Manual | Salesforce chat, form, phone |
| FAQ | 1-2 | Semi-Auto | Accordion content |
| Legal / Policy Pages | 5-6 | Automatic | Standard text content |
| My Profile | 1 | Manual | MFA, profile forms |
| Promotion FAQs | 1-2 | Semi-Auto | Standard Q&A format |
| Official Rules | 1-2 | Automatic | Legal text |
| **TOTAL** | **~40-50** | | |

### Migration Breakdown

| Migration Type | Page Count | Percentage |
|----------------|-----------|------------|
| Automatic (low complexity, standard content) | 8-10 | ~20% |
| Semi-Automatic (structured content, minor customization) | 18-25 | ~45% |
| Manual (dynamic, interactive, heavy logic) | 12-18 | ~35% |

---

## 4. Integrations Analysis

### Adobe Experience Cloud

| Integration | Type | Details | Complexity | Reference |
|-------------|------|---------|------------|-----------|
| **Adobe Experience Platform Launch** | Tag Management | `launch-598422f1c586.min.js` with 30+ extensions | Medium | All pages |
| **Adobe Analytics** | Analytics | AppMeasurement v2.27.0, Report Suite: `raiservices.global.prod`, Server: `raiservices.sc.omtrdc.net` | Medium | All pages |
| **Adobe Target** | Personalization | AT.js v2.11.7, View-based triggering per page (e.g., `secure:products`), Client Code: `raiservices` | High | All pages |
| **Adobe Audience Manager** | DMP | Audience segmentation module loaded via Launch | Medium | All pages |
| **Adobe Visitor ID Service** | Identity | Org: `02D9C50759DEA0920A495ED3@AdobeOrg`, Cross-brand visitor ID | Medium | All pages |
| **Adobe Client Data Layer** | Data Layer | v2.0.2, 73+ events tracked on homepage load | Medium | All pages |

### Authentication & Identity

| Integration | Type | Details | Complexity | Reference |
|-------------|------|---------|------------|-----------|
| **VIA/SSO Authentication** | Custom Auth | Cross-brand SSO via `securePage()`, shared across RAI sites | High | Login, all secure pages |
| **Multi-Factor Auth (MFA)** | Security | Email-based one-time passcode for profile access | High | My Profile |
| **Brand Site API** | REST API | `https://usapi.luckystrike.com`, Site Key: `lucky-strike` | High | Coupons, Profile, Auth |

### Loyalty & Rewards

| Integration | Type | Details | Complexity | Reference |
|-------------|------|---------|------------|-----------|
| **Loyalty Plus Platform** | Custom Platform | Rewards program: QR code scanning, points accumulation, gift card redemption. `loyaltyplus` clientlib loaded on all pages | High | Rewards pages, Homepage |
| **QR Code System** | Hardware/API | Physical pack QR codes linked to digital rewards points system | High | How It Works |

### Third-Party Services

| Integration | Type | Details | Complexity | Reference |
|-------------|------|---------|------------|-----------|
| **Google Maps API** | API | Interactive store locator with geocoding, geolocation, distance calculations | High | Store Locator |
| **Brightcove Video** | Embed/API | Account ID: `6134468300001`, video player for product showcases, content hub, and explainer videos | Medium | Products, American Originals, How It Works |
| **Knight Lab Juxtapose** | Embed | Before/after image comparison slider for historical pack designs | Low | History |
| **Salesforce Live Chat** | Embed | `bat-us.my.site.com/ESWLiveChat` for live customer support, Pre-chat API | High | Contact Us |
| **DoubleClick/Floodlight** | Ad Tracking | Google conversion tracking via network requests (DFA tags in Launch) | Medium | All pages |

### Performance & Monitoring

| Integration | Type | Details | Complexity | Reference |
|-------------|------|---------|------------|-----------|
| **Adobe Helix RUM** | Monitoring | `rum.hlx.page` Real User Monitoring | Low | All pages |
| **Service Worker** | Caching | Browser service worker support for offline/performance | Medium | All pages |
| **Google Site Verification** | SEO | Meta tag: `YV80medn3VNJ-CQn-yIO8jTOTx0Sm_tvq03rBDbLcAY` | Low | All pages |

### External Redirects

| Integration | Type | Details | Complexity | Reference |
|-------------|------|---------|------------|-----------|
| **Reynolds American Corporate** | Redirect | Sustainability link redirects to `reynoldsamerican.com/product-stewardship/` with UTM params | Low | Footer |
| **Own It Voice It** | Redirect | Tobacco Rights redirects to `ownitvoiceit.com` advocacy site | Low | Footer |

### Integration Count Summary

| Category | Count |
|----------|-------|
| Adobe Experience Cloud | 6 |
| Authentication & Identity | 3 |
| Loyalty & Rewards | 2 |
| Third-Party Services | 5 |
| Performance & Monitoring | 3 |
| External Redirects | 2 |
| **Total Integrations** | **21** |

---

## 5. Complex Use Cases & Observations

### 5.1 Loyalty Plus Rewards Program

**Complexity: VERY HIGH**
**Instances:** Pervasive across site (enrollment, dashboard, how-it-works, homepage CTAs, notification system)
**Where Found:** Rewards Enroll, How It Works, Homepage, Coupons, Notification bell

The Luckies Rewards program is a fully integrated loyalty platform:
- **QR Code Scanning:** Physical cigarette packs contain QR codes that link to digital points
- **Points Accumulation:** Multiple ways to earn - pack scans, site activities, promotions
- **Redemption:** Points redeemable for gift cards and mobile coupons
- **Dashboard:** Personal rewards dashboard with balance, activity history
- **Integration:** "Loyalty Plus" clientlib loaded on every page, influences header UI (notification bell count, "Join Rewards" / "Visit Rewards" button state)

**Why Complex:** Requires deep integration with a backend loyalty platform, physical product QR code system, points ledger, redemption catalog, and real-time balance display. The "Loyalty Plus" system appears to be a custom RAI platform, not a standard OOTB solution.

### 5.2 Interactive Sweepstakes Game

**Complexity: HIGH**
**Instances:** 1 active promotion ("Luckies' Garage")
**Where Found:** Sweepstakes page, Homepage promotion section

"Luckies' Garage" is a music-themed interactive game:
- Band/music simulation where users "hit notes" to win
- Instant win mechanics ($100 daily prizes, limited to 2/person/week)
- Weekly prizes ($2,000, limited to 1/person)
- Grand prize ($10,000)
- Runs 2/19/26 - 4/30/26

**Why Complex:** Gamified experiences require custom frontend development, backend prize management, instant win algorithms, rate limiting, and legal compliance. These are typically seasonal and change frequently.

### 5.3 American Originals Content Hub

**Complexity: HIGH**
**Instances:** 1 hub page + 15-25 article pages
**Where Found:** American Originals hub, individual article URLs

A full editorial content platform within the brand site:
- 25+ pieces of content with various formats (articles, videos, quizzes, interactive features)
- Brightcove video integration throughout
- Music/culture-themed content aligned with brand identity
- Content carousel on homepage promoting latest articles
- Each article page has its own template with hero, body, related content

**Why Complex:** High volume of content pages, multiple content formats, Brightcove video embeds, interactive elements (quizzes), and ongoing content production needs.

### 5.4 Brightcove Video Integration

**Complexity: MEDIUM-HIGH**
**Instances:** 15+ video instances across the site
**Where Found:** Products pages (video backgrounds), American Originals (content videos), How It Works (explainer video), Homepage

Brightcove is deeply integrated:
- Account ID: `6134468300001`
- Used for autoplay video backgrounds on product pages
- Content videos in editorial articles
- Explainer video for rewards program
- Multiple player instances per page (console shows 20+ "Ignoring already initialized player" warnings)

**Why Complex:** Video backgrounds require careful performance optimization. Brightcove player initialization needs proper lifecycle management. Content hub videos need individual embed configuration.

### 5.5 Notification Bell & Real-Time Offers

**Complexity: HIGH**
**Instances:** Present on all authenticated pages
**Where Found:** Header bar (top right)

Real-time notification system:
- Bell icon with badge count (shows "2" for available offers)
- Dropdown shows "Available Offers" with count and "Latest Activity" feed
- Count updates dynamically based on user's available coupons
- Links to Coupons page

**Why Complex:** Requires real-time or near-real-time API polling to update badge counts, personalization based on user state, and integration with the coupon management system.

### 5.6 Brand History Timeline with Interactive Elements

**Complexity: MEDIUM-HIGH**
**Instances:** 1 page with 7 eras
**Where Found:** History/About page

Rich interactive timeline:
- Knight Lab Juxtapose before/after slider at top
- 7 era sections (1871-2020s), each with image carousel
- Interactive poll with image-based radio buttons
- Historical narrative with era-specific typography

**Why Complex:** Combines multiple interactive libraries (Juxtapose, carousels), requires careful responsive handling, and the poll needs backend vote tallying.

### 5.7 Personalized Coupon System

**Complexity: HIGH**
**Instances:** Coupons page + notification integration
**Where Found:** Coupons, Header notification, Homepage

- Personalized greeting with user's first name
- Dynamic offer count ("You've got offers!")
- Year-to-date savings tracker ("$0 Saved So Far in 2026")
- "View Coupon" button for coupon reveal
- 4-step in-store redemption with 5-minute expiry timer
- Integration with store locator for retailer selection

**Why Complex:** Deep personalization, real-time coupon availability, in-store redemption flow with time-limited codes, and integration with retailer acceptance systems.

### 5.8 Console Errors & Technical Debt

**Observed Issues:**
- `TypeError: w[l].push is not a function` - Occurs on every page
- `Adobe Client Data Layer v2.0.2 has already been imported/initialized` - Double initialization
- `Failed to load resource: 404` - Missing API endpoints
- `Refused to execute script from 'undefined'` - Script source failures on Contact page
- `Tabs: container utilities not available` (on some pages) - AEM Core Components issue
- 20+ `VIDEOJS: Ignoring already initialized player` warnings on American Originals page

**Migration Opportunity:** These errors indicate significant technical debt that would be resolved with a clean EDS implementation.

### 5.9 CMS Stage URL Leak

**Observation:** The Federal Court notice on the homepage links to `https://cms-stage.raimktg.com/editor.html/content/newport/en/secure.html#health-effects` - this is an internal AEM Author URL that should not be exposed in production.

---

## 6. Migration Estimates

### Effort Breakdown by Category

#### A. Design System & Global Styles
| Task | Effort (Person-Days) |
|------|---------------------|
| Design token extraction (colors, typography, spacing) | 3 |
| Global CSS variables and responsive framework | 3 |
| Font integration (custom brand fonts) | 1 |
| Surgeon General's warning component | 0.5 |
| Federal Court notice banner | 0.5 |
| **Subtotal** | **8** |

#### B. Navigation & Chrome
| Task | Effort (Person-Days) |
|------|---------------------|
| Header with rewards button & notification bell | 4 |
| Notification dropdown with offers count & activity | 3 |
| Mobile hamburger navigation with submenu | 2 |
| Footer (two-row with social, warning) | 1.5 |
| **Subtotal** | **10.5** |

#### C. Page Templates
| Task | Effort (Person-Days) |
|------|---------------------|
| Homepage layout (multi-section, personalized) | 3 |
| Products listing with video carousel | 2.5 |
| Product detail pages | 1.5 |
| American Originals content hub | 3 |
| Article/content page template | 2 |
| Sweepstakes/promotion template | 2 |
| Brand history timeline | 2.5 |
| Store Locator page | 1 |
| Coupons page | 2 |
| SMS signup page | 1 |
| Rewards enrollment page | 1 |
| How It Works page | 1 |
| Contact Us page | 1 |
| FAQ pages | 1 |
| Legal/policy template | 0.5 |
| Profile page | 1.5 |
| Login/registration page | 2 |
| **Subtotal** | **28.5** |

#### D. Block Development
| Task | Effort (Person-Days) |
|------|---------------------|
| Video background hero block | 3 |
| Content carousel with article cards | 3 |
| Product carousel with labeled pagination | 3 |
| Image carousel (history eras) | 2 |
| Dual CTA card section | 1.5 |
| Sweepstakes promotion banner | 2 |
| Rewards/coupon promotional cards | 2 |
| Welcome banner (personalized) | 1 |
| Brand statement section | 1 |
| Step-by-step instructions (rewards/coupons) | 1.5 |
| Accordion/FAQ block | 1.5 |
| Store locator CTA block | 0.5 |
| Article card (content hub) | 1.5 |
| Timeline era section | 2 |
| Interactive poll block | 2 |
| Prize display section | 1 |
| Product detail section | 1 |
| Contact multi-channel block | 1.5 |
| SMS signup form block | 1 |
| Login/registration form block | 2 |
| Savings tracker widget | 1 |
| **Subtotal** | **35** |

#### E. Integrations
| Task | Effort (Person-Days) |
|------|---------------------|
| Age gate/VIA SSO authentication | 5 |
| MFA implementation | 3 |
| Brand Site API integration | 4 |
| Loyalty Plus rewards integration | 8 |
| QR code scanning system interface | 3 |
| Notification bell real-time system | 4 |
| Personalized coupon system | 5 |
| Google Maps store locator | 3 |
| Brightcove video player integration | 3 |
| Knight Lab Juxtapose | 1 |
| Salesforce Live Chat | 2 |
| Adobe Analytics/Launch migration | 3 |
| Adobe Target personalization | 2 |
| DoubleClick conversion tracking | 1 |
| **Subtotal** | **47** |

#### F. Content Migration
| Task | Effort (Person-Days) |
|------|---------------------|
| Content authoring for ~40-50 pages | 6 |
| Article content migration (15-25 articles) | 4 |
| Image/video asset migration | 2 |
| Legal content migration (5-6 pages) | 1 |
| FAQ and product content | 1 |
| Historical timeline content | 1 |
| **Subtotal** | **15** |

#### G. Interactive Features
| Task | Effort (Person-Days) |
|------|---------------------|
| Sweepstakes game development | 8 |
| Interactive poll system | 2 |
| Quiz functionality (content hub) | 3 |
| **Subtotal** | **13** |

#### H. Testing & QA
| Task | Effort (Person-Days) |
|------|---------------------|
| Cross-browser testing | 3 |
| Mobile responsive testing | 3 |
| Accessibility audit (WCAG 2.1 AA) | 3 |
| Performance optimization (Core Web Vitals) | 3 |
| Integration testing (auth, rewards, coupons, maps, video) | 5 |
| Sweepstakes/game testing | 2 |
| UAT support | 3 |
| **Subtotal** | **22** |

### Summary

| Category | Low Estimate | High Estimate |
|----------|-------------|---------------|
| Design System & Global Styles | 6 | 10 |
| Navigation & Chrome | 8 | 13 |
| Page Templates | 24 | 34 |
| Block Development | 30 | 42 |
| Integrations | 40 | 56 |
| Content Migration | 12 | 18 |
| Interactive Features | 10 | 16 |
| Testing & QA | 18 | 26 |
| **TOTAL** | **148** | **215** |

### Risk-Adjusted Estimate

| Scenario | Person-Days | Calendar Weeks (2-person team) |
|----------|-------------|-------------------------------|
| **Optimistic** (smooth integrations, minimal scope changes) | 148 | 15-16 weeks |
| **Most Likely** (standard complexity, moderate rework) | 180 | 18-20 weeks |
| **Pessimistic** (rewards platform complexity, game redevelopment, content volume) | 215 | 22-24 weeks |

### Key Risk Factors

1. **Loyalty Plus Platform:** The rewards system is deeply integrated and likely requires significant API coordination. QR code scanning from physical packs adds hardware/software complexity.
2. **Sweepstakes Game:** Interactive games require custom development, prize management backend, and legal compliance. Games change seasonally, requiring a flexible framework.
3. **Brightcove Video Volume:** 15+ video instances with video backgrounds need careful performance optimization to maintain Core Web Vitals.
4. **Content Hub Volume:** 25+ articles with various formats (text, video, quiz, interactive) require diverse content migration strategies.
5. **Notification System:** Real-time offer counting and activity feed requires persistent API integration.
6. **Cross-Brand SSO:** Authentication coordination across multiple RAI brands involves multiple stakeholders.

### Comparison to Other RAI Brand Sites

| Site | Pages | Components | Integrations | Estimated Days |
|------|-------|------------|-------------|---------------|
| americanspirit.com | ~25-30 | ~35 | ~25 | 120-170 |
| camel.com | ~30-40 | ~40 | ~30 | 150-210 |
| camelsnus.com | ~20-25 | ~30 | ~22 | 100-140 |
| vusevapor.com | ~48-55 | ~40 | ~32 | 195-310 |
| cougardips.com | ~18-20 | ~30 | ~19 | 77-110 |
| **luckystrike.com** | **~40-50** | **~43** | **~21** | **148-215** |

LuckyStrike.com is the **second most complex** site in the RAI portfolio (after vusevapor.com), primarily due to the Loyalty Plus rewards program, interactive sweepstakes, Brightcove video integration, and extensive content hub. However, its integration count is moderate compared to vusevapor.com, as the complexity lies more in feature depth than in the breadth of third-party services.

---

## Appendix: Screenshots

### Screenshot 1: Login Page
![Login](/workspace/site-analysis/screenshots/lucky-01-login.png)

### Screenshot 2: Homepage
![Homepage](/workspace/site-analysis/screenshots/lucky-02-homepage.png)

### Screenshot 3: Products
![Products](/workspace/site-analysis/screenshots/lucky-03-products.png)

### Screenshot 4: American Originals (Content Hub)
![American Originals](/workspace/site-analysis/screenshots/lucky-04-american-originals.png)

### Screenshot 5: Sweepstakes (Luckies' Garage)
![Sweepstakes](/workspace/site-analysis/screenshots/lucky-05-sweepstakes.png)

### Screenshot 6: History / About Us
![History](/workspace/site-analysis/screenshots/lucky-06-history.png)

### Screenshot 7: Store Locator
![Store Locator](/workspace/site-analysis/screenshots/lucky-07-store-locator.png)

### Screenshot 8: Coupons
![Coupons](/workspace/site-analysis/screenshots/lucky-08-coupons.png)

### Screenshot 9: SMS Signup
![SMS](/workspace/site-analysis/screenshots/lucky-09-sms.png)

### Screenshot 10: Rewards Enrollment
![Rewards Enroll](/workspace/site-analysis/screenshots/lucky-10-rewards-enroll.png)

### Screenshot 11: How It Works (Rewards)
![How It Works](/workspace/site-analysis/screenshots/lucky-11-how-it-works.png)

### Screenshot 12: Product Detail (Non-Menthol)
![Product Detail](/workspace/site-analysis/screenshots/lucky-12-product-detail.png)

### Screenshot 13: Contact Us
![Contact Us](/workspace/site-analysis/screenshots/lucky-13-contact-us.png)
