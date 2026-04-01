# My Grizzly (mygrizzly.com) — Comprehensive Site Analysis

**Prepared for:** Adobe Experience Manager Edge Delivery Services Migration Assessment
**Analysis Date:** March 31, 2026
**Analyst:** Adobe Professional Services

---

## Executive Summary

My Grizzly (mygrizzly.com) is the consumer brand website for **Grizzly** smokeless tobacco products, owned by **American Snuff Company, LLC**, a subsidiary of **Reynolds American Inc. (RAI)**, part of **British American Tobacco (BAT)**. The site is built on **Adobe Experience Manager (AEM) as a Cloud Service** using freeform page templates with extensive custom components.

Grizzly is the **most feature-rich and complex** RAI brand website analyzed to date. It includes a full-featured content hub (Grizz List articles with likes/comments), interactive quizzes (Grizz Quiz), a conservation program (Outdoor Corps with 21 projects and 15 expeditions), advanced product catalog with comparison and filtering (20 product variants), personalized coupons, SMS marketing, and a store locator. The site serves as an age-gated (21+) loyalty and engagement platform for adult moist snuff and snus consumers.

**Key Metrics:**
- **Estimated Pages:** ~120+ (including 21 project detail pages, 15 expedition pages, 15+ Grizz List articles, 15+ quizzes, 20 product detail pages, and utility pages)
- **Templates Identified:** 15
- **Components/Blocks Cataloged:** 48
- **Third-Party Integrations:** 16+
- **Migration Complexity:** Very High
- **Estimated Migration Effort:** 120–180 person-days

---

## 1. Templates Inventory

### Template 1: Homepage
- **URL Pattern:** `/secure.html`
- **Description:** Video hero with Brightcove player, promotional content cards (coupon CTA, expedition promo, Best By date campaign, expedition results, Grizz Quiz promo), personalized greeting
- **Distinguishing Features:** Full-width video hero, multi-card promotional grid, dynamic personalization, animated transitions
- **Occurrence:** 1 page

![Homepage](screenshots/grizzly2-01-homepage.png)

### Template 2: Products Listing (Moist Snuff)
- **URL Pattern:** `/secure/products/all-products.html`
- **Description:** Product catalog with advanced multi-axis filtering (Style: Pouches/Dark; Cut: Long Cut/Extra Long Cut/Fine Cut/Snuff/Wide Cut; Flavor: Wintergreen/Straight/Mint/Natural), product grid with comparison checkboxes, "Select Another Product" comparison trigger
- **Distinguishing Features:** Radio button filter groups, product comparison feature with checkbox selection, 17 moist snuff products displayed
- **Occurrence:** 1 page

![Products](screenshots/grizzly2-02-products.png)

### Template 3: Products Listing (Spitfree/Snus)
- **URL Pattern:** `/secure/products/spitfree.html`
- **Description:** Spitfree sub-brand product catalog with hero banner, 3 snus product cards (Arctic Blue, Wintergreen, Natural), sub-brand tabs (Moist Snuff / Spitfree)
- **Distinguishing Features:** Different warning label ("SNUS" vs "MOIST SNUFF"), sub-brand hero with tagline "Real tobacco pouches. No spit cup required.", product comparison button
- **Occurrence:** 1 page

![Spitfree](screenshots/grizzly2-08-spitfree.png)

### Template 4: Product Detail
- **URL Pattern:** `/secure/products/all-products/{product-slug}.html`
- **Description:** Individual product page with product name, description, flavor profile visualization (Tobacco Taste, Intensity, Palate on 1–10 scales), tobacco blend breakdown (American/Brazilian percentages), cut type with icon, product comparison dropdowns (20 products), "Pairs Well With" lifestyle section, and related products
- **Distinguishing Features:** Interactive flavor profile scales, tobacco blend percentages, "Pairs Well With" tags (e.g., "Old Leather", "Whiskey", "Outlawin'"), product comparison with dual dropdown selects and "Add another product" button
- **Occurrence:** ~20 pages (17 moist snuff + 3 snus)

![Product Detail](screenshots/grizzly2-09-product-detail.png)

### Template 5: Coupons
- **URL Pattern:** `/secure/coupons.html`
- **Description:** Personalized coupon dashboard with user greeting ("NIHAR, YOU HAVE 15 Coupons Available"), MAIL/MOBILE tabs with counts, coupon cards, "HOW IT WORKS" button, FAQ button, yearly claimed savings tracker ("$0.00 YOUR 2026 CLAIMED SAVINGS*")
- **Distinguishing Features:** Personalized coupon count, mail vs. mobile tabs, savings tracker, dynamic coupon loading
- **Occurrence:** 1 page

![Coupons](screenshots/grizzly2-03-coupons.png)

### Template 6: Explore / Grizz List Article
- **URL Pattern:** `/secure/explore/grizz-list/{year}/{article-slug}.html`
- **Description:** Content hub article with full-width hero image, article title, numbered list content (e.g., "Top Five States According To Texans"), social engagement (like count, comment count), previous/next article navigation, category filter sidebar (All, Food, Drinking, Outdoors, Sharks, Rules & Advice, Best Worst), article grid with thumbnails
- **Distinguishing Features:** Like button with count (196 likes), comment button with count (1 comment), left/right arrow navigation between articles, category-based filtering, content spanning 2019–2026
- **Occurrence:** 15+ pages

![Explore](screenshots/grizzly2-04-explore.png)

### Template 7: Grizz Quiz
- **URL Pattern:** `/secure/explore/grizz-quiz/{year}/{quiz-slug}.html`
- **Description:** Interactive quiz with hero section, 10-question format with image per question, multiple-choice answers, attempt counter, like/comment engagement, previous/next quiz navigation, quiz catalog grid with category filtering (All, Sports, Wildlife, Survival, Cars & Stuff, Fun Stuff) and attempt counts per quiz
- **Distinguishing Features:** Multi-step interactive quiz engine, restart button, attempt tracking (e.g., "Attempted 32 times", "12264 attempts"), quiz catalog with 15+ quizzes spanning 2025–2026
- **Occurrence:** 15+ pages

![Grizz Quiz](screenshots/grizzly2-14-grizz-quiz.png)

### Template 8: Outdoor Corps — Conservation Projects Listing
- **URL Pattern:** `/secure/outdoor-corps/projects.html`
- **Description:** Video hero (Brightcove), introductory heading, grid of 21 conservation project cards with thumbnail images, titles, descriptions, and "Learn More" CTAs
- **Distinguishing Features:** Large conservation program with 21 projects spanning multiple years and geographies (Alaska, Idaho, Montana, Florida, Kentucky, California, Arkansas, Wyoming, Colorado, Texas, North Carolina, Utah, New Mexico, Nebraska)
- **Occurrence:** 1 page

### Template 9: Outdoor Corps — Conservation Project Detail
- **URL Pattern:** `/secure/outdoor-corps/projects/{project-slug}.html`
- **Description:** Full-width video hero (Brightcove), project title and description, embedded video player with play button, project map image, photo carousel (multi-slide), related projects grid
- **Distinguishing Features:** Dual video content (hero + embedded), image carousel with slide navigation, project map visualization, related projects cross-linking
- **Occurrence:** 21 pages

![Project Detail](screenshots/grizzly2-15-project-detail.png)

### Template 10: Outdoor Corps — Expeditions Listing
- **URL Pattern:** `/secure/outdoor-corps/expeditions.html`
- **Description:** Video hero (Brightcove), introductory heading, grid of 15 expedition cards with thumbnails, titles, descriptions, and CTAs spanning 2016–2026
- **Distinguishing Features:** Expedition cards with varied CTA labels ("Learn More", "Let's See It", "Let's Hunt", "Watch", "Find Out"), chronological content from 2016 to 2026
- **Occurrence:** 1 page

### Template 11: Outdoor Corps — Expedition Detail
- **URL Pattern:** `/secure/outdoor-corps/expeditions/{expedition-slug}.html`
- **Description:** Individual expedition story pages with video, narrative content, and imagery (similar structure to project detail)
- **Occurrence:** 15 pages

### Template 12: Store Locator
- **URL Pattern:** `/secure/store-locator.html`
- **Description:** Google Maps integration with geolocation ("Find Me"), zip code search, product sub-tabs (Moist Snuff / SPITFREE with separate store locator), "Filter by Product" button, numbered store list with addresses, distances, "Get Directions" links, expandable product availability, "Load More" pagination, map with numbered pins
- **Distinguishing Features:** Dual product category store locators (Moist Snuff vs Spitfree), Google Maps Advanced Markers API, "Some styles may not be available in your state or local jurisdiction" disclaimer
- **Occurrence:** 2 pages (Moist Snuff + Spitfree)

### Template 13: SMS Signup
- **URL Pattern:** `/secure/sms.html`
- **Description:** Hero image with SMS benefits list (Latest offers, New giveaways, Product info, Stuff we think is cool), phone number input, welcome offer callout ("$2.00 off two cans of Grizzly"), TCPA consent checkbox with detailed legal language
- **Distinguishing Features:** Welcome coupon incentive, comprehensive TCPA/legal consent language, R.J. Reynolds + American Snuff Company + affiliated entities consent
- **Occurrence:** 1 page

![SMS](screenshots/grizzly2-10-sms.png)

### Template 14: My Profile (MFA-Protected)
- **URL Pattern:** `/secure/my-profile.html`
- **Description:** Multi-factor authentication gate (passcode sent to email), profile management with "Products" and "Custom Cans" tabs visible
- **Distinguishing Features:** MFA passcode verification, "Custom Cans" feature (personalized can design), profile preferences management
- **Occurrence:** 1 page

![Profile MFA](screenshots/grizzly2-11-profile-mfa.png)

### Template 15: Footer/Utility Pages
- **URL Pattern:** `/secure/footer-links/{page}.html`
- **Description:** Contact Us (Chat + Email + Call), FAQ (5 sections, 15 Q&As with accordion), Tobacco Rights, Site Requirements, Terms of Use, Privacy Policy, Text Messaging T&C
- **Distinguishing Features:** Contact Us has live chat widget (Prechat API), email form with 7 topic categories, phone number (1-866-843-0636); FAQ uses accordion pattern with anchor link navigation; legal pages are text-heavy
- **Occurrence:** 7+ pages

![Contact Us](screenshots/grizzly2-12-contact-us.png)

![FAQ](screenshots/grizzly2-13-faq.png)

---

## 2. Blocks / Components Catalog

### Global Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 1 | **Health Warning Banner** | Fixed top banner with product category label ("MOIST SNUFF", "SNUS", "Moist Snuff and Snus") and FDA-mandated warning: "WARNING: This product can cause mouth cancer." Dynamic category based on page context | Low |
| 2 | **Global Header/Navigation** | Grizzly logo with link to homepage, hamburger menu toggle, 6-item main nav (Explore, Outdoor Corps, Products, Coupons, Store Locator, My Profile) with submenu buttons for first 4 items, dynamic coupon badge count ("14") on Coupons link | High |
| 3 | **Global Footer** | Two-row link structure: Row 1 (Home, Products, Coupons, My Profile, Logout), Row 2 (Contact Us, FAQ, Tobacco Rights, Site Requirements, Terms of Use, Privacy Policy, Text Messaging T&C), social icons (Facebook, Instagram, SMS) | Medium |
| 4 | **Age Gate / VIA SSO** | Cross-brand RAI age verification with `viasso=true` parameter, 21+ authentication requirement, redirect to `/secure/` path after verification | High |
| 5 | **MFA Verification** | Multi-factor authentication overlay with passcode sent to email, passcode input field, "Continue" button, resend code messaging | High |

### Homepage Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 6 | **Video Hero (Brightcove)** | Full-width video hero with Brightcove player (Account: 5141850720001), auto-play background video, overlay content area | High |
| 7 | **Promotional Card Grid** | Multi-card promotional layout with varied card types: coupon CTA ("SAVE $5 ON ANY FIVE TINS"), expedition promo, product campaign ("DIP FRESH EVERY TIME"), expedition results, quiz promo | Medium |
| 8 | **Coupon CTA Card** | Styled card with coupon offer headline, supporting text, and CTA button linking to coupons page | Low |
| 9 | **Expedition Promo Card** | Card featuring expedition imagery (e.g., "Expedition 2026 Alaska"), descriptive text, and CTA to expedition detail | Low |
| 10 | **Best By Date Campaign Card** | Marketing campaign card for "DIP FRESH EVERY TIME" Best By date initiative with product imagery | Low |
| 11 | **Grizz Quiz Promo Card** | Card promoting latest Grizz Quiz with quiz title and CTA to quiz page | Low |

### Product Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 12 | **Product Filter Panel** | Multi-axis radio button filter groups: Style (Pouches, Dark), Cut (Long Cut, Extra Long Cut, Fine Cut, Snuff, Wide Cut), Flavor (Wintergreen, Straight, Mint, Natural) — filters product grid dynamically | High |
| 13 | **Product Card (with Comparison)** | Product image, product name, checkbox for comparison selection, link to product detail | Medium |
| 14 | **Product Comparison Trigger** | "Select Another Product" button that activates when comparison checkboxes are selected | Medium |
| 15 | **Product Sub-Brand Tabs** | Toggle between "Moist Snuff" and "SPITFREE" product categories, persists as navigation between product listing pages | Low |
| 16 | **Flavor Profile Visualization** | Three horizontal scale visualizations (Tobacco Taste: Mild–Bold, Intensity: Subtle–Strong, Palate: Less Sweet–More Sweet) with numeric ratings on 1–10 scale | High |
| 17 | **Tobacco Blend Breakdown** | Percentage display of American vs Brazilian tobacco with descriptive modals/tooltips | Medium |
| 18 | **Cut Type Display** | Icon-based display of product cut type (Long Cut, Fine Cut, etc.) with modal/tooltip details | Medium |
| 19 | **Product Comparison Widget** | Dual dropdown selects populated with all 20 products, "Add another product" button, "Compare Products" action button | High |
| 20 | **Pairs Well With** | Lifestyle association tags for product (e.g., "Old Leather", "Whiskey", "Outlawin'", "Winning at Poker", "Homesteading") | Low |
| 21 | **Related Products** | Horizontal card row showing related product links with product names | Low |

### Coupon Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 22 | **Personalized Greeting** | User-specific welcome with first name and available coupon count ("NIHAR, YOU HAVE 15 Coupons Available") | Medium |
| 23 | **Coupon Tab Toggle** | MAIL/MOBILE tabs with respective counts (MAIL: 1, MOBILE: 14) | Medium |
| 24 | **Coupon Card** | Individual coupon display with offer details, claim mechanism, terms | Medium |
| 25 | **Savings Tracker** | Annual claimed savings counter ("$0.00 YOUR 2026 CLAIMED SAVINGS*") | Low |
| 26 | **Coupon Info Buttons** | "HOW IT WORKS" and "FAQ" buttons for coupon usage guidance | Low |

### Explore / Content Hub Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 27 | **Article Hero** | Full-width background image with article category label ("GRIZZ LIST"), large title text, "Saddle Up" CTA button | Medium |
| 28 | **Social Engagement Bar** | Previous/next arrow navigation, comment button with count, like button with count (e.g., 196 likes) | High |
| 29 | **Numbered Article Content** | Numbered list display (5, 4, 3, 2, 1 countdown format) with heading and description per item | Medium |
| 30 | **Category Filter Sidebar** | Vertical filter with category radio buttons (All, Food, Drinking, Outdoors, Sharks, Rules & Advice, Best Worst) | Medium |
| 31 | **Article Grid** | Thumbnail-based article card grid with titles, 3-column layout, spanning multiple years | Medium |

### Grizz Quiz Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 32 | **Quiz Hero** | "Grizz Quiz" label, quiz title, "Start Quiz" button, attempt counter ("Attempted 32 times") | Medium |
| 33 | **Quiz Question Card** | Question number indicator ("Question 1 of 10"), question image, question text, multiple-choice answer listItems, next button, restart link | Very High |
| 34 | **Quiz Category Filter** | Radio button categories (All, Sports, Wildlife, Survival, Cars & Stuff, Fun Stuff) | Medium |
| 35 | **Quiz Catalog Grid** | Quiz card grid with thumbnail images, titles, attempt counts (e.g., "12264 attempts") | Medium |

### Outdoor Corps Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 36 | **Conservation Project Card** | Thumbnail image, project title, short description, CTA button with varied labels | Low |
| 37 | **Expedition Card** | Thumbnail image, expedition title, description, CTA with varied labels | Low |
| 38 | **Project Detail Video** | Embedded video player with play button overlay and HD indicator | High |
| 39 | **Project Map** | Static map image showing project location | Low |
| 40 | **Photo Carousel** | Multi-slide image carousel with navigation (e.g., "Slide 1 of 3") | High |
| 41 | **Related Projects Grid** | Grid of related conservation project cards at bottom of detail page | Medium |

### Store Locator Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 42 | **Store Search** | Zip code input, "Find Me" geolocation button, "Find Stores" submit button, "Filter by Product" toggle | High |
| 43 | **Store Results List** | Numbered store cards with store name, address, "Get Directions" link (Google Maps), distance in miles, expandable product availability | High |
| 44 | **Google Maps Embed** | Interactive Google Maps with numbered markers, Map/Satellite toggle, fullscreen, Street View pegman, zoom controls | Very High |

### SMS & Contact Components

| # | Component | Description | Complexity |
|---|-----------|-------------|------------|
| 45 | **SMS Signup Form** | Hero image, benefits list, phone number input, welcome offer callout, TCPA consent checkbox with legal text, "Sign Up" button | High |
| 46 | **Contact Channel Cards** | Three contact options: Chat (live chat widget), Email (topic dropdown + message textarea), Call (toll-free number) | High |
| 47 | **FAQ Accordion** | Section-based accordion with 5 categories, 15 Q&As, expand/collapse with icon toggle, anchor link navigation | Medium |
| 48 | **Custom 404 Page** | "Well, this is embarrassing." heading, description, "Go Home" button | Low |

---

## 3. Page Counts by Template

| Template | Estimated Page Count | Notes |
|----------|---------------------|-------|
| Homepage | 1 | Video hero, promotional cards |
| Products Listing (Moist Snuff) | 1 | 17 products with advanced filtering |
| Products Listing (Spitfree/Snus) | 1 | 3 snus products |
| Product Detail | ~20 | 17 moist snuff + 3 snus variants |
| Coupons | 1 | Personalized coupon dashboard |
| Explore / Grizz List Article | 15+ | Content articles spanning 2019–2026 |
| Grizz Quiz | 15+ | Interactive quizzes spanning 2025–2026 |
| Outdoor Corps — Projects Listing | 1 | 21 conservation projects |
| Outdoor Corps — Project Detail | 21 | Individual project pages |
| Outdoor Corps — Expeditions Listing | 1 | 15 expeditions |
| Outdoor Corps — Expedition Detail | 15 | Individual expedition pages |
| Store Locator | 2 | Moist Snuff + Spitfree |
| SMS Signup | 1 | SMS marketing enrollment |
| My Profile | 1 | MFA-protected profile management |
| Footer/Utility Pages | 7+ | Contact Us, FAQ, legal pages |
| **TOTAL** | **~120+** | **Most complex RAI brand site** |

---

## 4. Integrations & Third-Party Services Analysis

### Adobe Experience Cloud Stack

| Integration | Details | Shared Across RAI |
|-------------|---------|-------------------|
| **Adobe Launch (DTM)** | `launch-EN66d1505d231e4d7a8fc8c95533aae9b5.min.js` | Yes — identical across all RAI brands |
| **Adobe Analytics** | AppMeasurement v2.22.4, Report Suite: `raiservices.global.prod`, Server: `raiservices.sc.omtrdc.net` | Yes |
| **Adobe Target** | v2.11.4, personalization and A/B testing | Yes |
| **Adobe Client Data Layer** | v5.4.0, standardized data layer | Yes |
| **Adobe Audience Manager** | Integrated via Launch, audience segmentation | Yes |
| **Adobe Org ID** | `02D9C50759DEA0920A495ED3@AdobeOrg` | Yes |
| **Adobe Helix RUM** | Real User Monitoring active | Yes |

### Video Platform

| Integration | Details |
|-------------|---------|
| **Brightcove** | Account: `5141850720001` (shared with grizzlynicotinepouches.com), video hero on Homepage, Outdoor Corps project listing, expedition listing, and all project/expedition detail pages |

### Mapping & Location

| Integration | Details |
|-------------|---------|
| **Google Maps JavaScript API** | Advanced Markers API, Map/Satellite views, Street View, Directions integration via `maps.google.com/maps/dir/` |
| **Google Site Verification** | `lRWhK0feFuhSnDevxlkJtAPjph8in7UIV30Tmb0EwRw` |

### Advertising & Tracking

| Integration | Details |
|-------------|---------|
| **DoubleClick/Floodlight** | `DC-9818726` via Google Tag Manager — conversion tracking for ad campaigns (unique to mygrizzly.com among RAI brands analyzed) |
| **MiQ Digital** | `honestclick.miqdigital.com` — programmatic advertising tracking (connection failures in test environment; unique to mygrizzly.com) |
| **Vindico Suite** | `mpp.vindicosuite.com` — video ad verification and measurement (timeouts in test environment; unique to mygrizzly.com) |

### Authentication & API

| Integration | Details |
|-------------|---------|
| **RAI VIA/SSO** | Cross-brand authentication with `viasso=true` parameter, 21+ age verification, MFA passcode via email |
| **Brand API** | `api.mygrizzly.com`, Brand key: `grizzly` — product data, coupons, store locator, user profile, quiz data |
| **Service Worker** | `resource-cache-service-worker.js` — client-side resource caching for performance |

### Social & Communication

| Integration | Details |
|-------------|---------|
| **Facebook** | `facebook.com/grizzlysmokeless` — social link in footer |
| **Instagram** | `instagram.com/grizzlysmokeless` — social link in footer |
| **SMS Marketing** | In-app SMS signup with TCPA consent, welcome coupon incentive ($2.00 off), recurring marketing messages |
| **Live Chat** | Prechat API integration on Contact Us page, "Hello, have a question? Let's chat." widget |

### AEM Infrastructure

| Component | Details |
|-----------|---------|
| **AEM Version** | AEM as a Cloud Service |
| **Client Libraries** | `reynoldsamerican-aem-base/clientlibs` + `grizzly/clientlibs` |
| **Build Hash** | `05fb5805407d527c8b8f0de84cbfd3709d111022` (2026-03-19T18:56:25+0000) |
| **Template Type** | Freeform page template |
| **Core Components** | Tabs, Accordion, Carousel (with container utility warnings) |

---

## 5. Complex Use Cases & Observations

### 5.1 Grizz List Content Hub — Social Engagement Platform

The Grizz List is a full-featured content hub with article-level social engagement:
- **Like System:** Articles display like counts (e.g., 196 likes) with clickable like button
- **Comment System:** Articles display comment counts with clickable comment button
- **Sequential Navigation:** Previous/next arrow buttons navigate between articles chronologically
- **Category Filtering:** 7 categories (All, Food, Drinking, Outdoors, Sharks, Rules & Advice, Best Worst) filter the article grid
- **Multi-Year Content:** Articles span 2019–2026, indicating a long-running content program
- **Migration Challenge:** The social engagement layer (likes, comments) requires backend API integration. The sequential navigation implies an ordered content index. Category filtering needs a taxonomy system. This is the most complex content feature across all RAI brands analyzed.

### 5.2 Grizz Quiz — Interactive Quiz Engine

The Grizz Quiz system is a fully interactive quiz platform:
- **10-Question Format:** Each quiz has 10 questions with images and multiple-choice answers
- **State Management:** Progress tracking (Question X of 10), restart capability
- **Attempt Tracking:** Global attempt counts per quiz (e.g., "12264 attempts") indicate server-side tracking
- **Category System:** 6 categories (All, Sports, Wildlife, Survival, Cars & Stuff, Fun Stuff)
- **Engagement:** Like/comment buttons on quiz pages, previous/next quiz navigation
- **Volume:** 15+ quizzes across 2025–2026 with active community engagement
- **Migration Challenge:** Requires custom interactive block with multi-step state management, server-side attempt tracking, and result calculation logic. Cannot be replicated with static EDS blocks alone.

### 5.3 Advanced Product Filtering & Comparison

The product catalog features the most sophisticated filtering of any RAI brand:
- **Multi-Axis Filtering:** 4 filter dimensions (Style, Cut, Flavor, and implicit product type) with radio button groups
- **Product Comparison:** Checkbox-based product selection from the listing page, plus dropdown-based comparison on detail pages with up to 3 products
- **Rich Product Detail:** Flavor profile scales (3 dimensions on 1–10 scales), tobacco blend percentages, cut type icons with modals, "Pairs Well With" lifestyle tags
- **20 Product Variants:** 17 moist snuff + 3 snus products, each with unique detail pages
- **Migration Challenge:** The filtering and comparison features require significant client-side JavaScript. The flavor profile visualizations need custom CSS for scale rendering. Product data appears to come from the Brand API.

### 5.4 Outdoor Corps Conservation Program

The Outdoor Corps is an extensive conservation and outdoor engagement program:
- **Conservation Projects (21):** Each with dedicated detail page featuring dual Brightcove videos, project map, photo carousel, and narrative content. Projects span Alaska, Idaho, Montana, Florida, Kentucky, California, Arkansas, Wyoming, Colorado, Texas, North Carolina, Utah, New Mexico, and Nebraska.
- **Expeditions (15):** Each with dedicated story page. Expeditions span 2016–2026 covering fishing, hunting, and outdoor experiences.
- **Video-Heavy Content:** Every project listing, expedition listing, and detail page features Brightcove video heroes
- **Migration Challenge:** 36 detail pages with rich media, carousels, embedded videos, and maps. The volume of Brightcove video embeds requires careful media migration planning.

### 5.5 Custom Cans Feature (Profile)

The My Profile page reveals a "Custom Cans" tab alongside "Products", suggesting a personalization feature where users can design or customize their Grizzly can graphics. This feature:
- Is behind MFA authentication
- Was not fully explorable due to MFA gate
- Represents a unique interactive customization tool not seen on other RAI brands
- **Migration Challenge:** Custom can designer would require a dedicated interactive block with likely canvas/image manipulation capabilities

### 5.6 Personalized Coupon System with Badge Notifications

The coupon system shows sophisticated personalization:
- **Navigation Badge:** Live coupon count ("14") displayed as a badge on the Coupons nav link — requires dynamic data injection into the header
- **Personalized Dashboard:** User-specific greeting with name and available coupon count
- **Mail vs Mobile Channels:** Separate tabs for physical mail coupons vs mobile coupons with independent counts
- **Savings Tracking:** Annual cumulative savings tracker
- **Migration Challenge:** The navigation badge count requires header-level API integration. The personalized coupon dashboard needs authenticated API calls to the Brand API.

### 5.7 Dual Product Category Architecture

Grizzly uniquely maintains two distinct product lines with separate experiences:
- **Moist Snuff:** 17 products with advanced filtering (4 axes), warning label "MOIST SNUFF"
- **Spitfree (Snus):** 3 products with simplified listing, warning label "SNUS", separate sub-brand identity with distinct hero
- **Store Locator Split:** Separate store locator pages/tabs for Moist Snuff and Spitfree
- **Dynamic Warning Labels:** The health warning banner dynamically changes between "MOIST SNUFF", "SNUS", and "Moist Snuff and Snus" based on page context
- **Migration Challenge:** The dynamic warning label system and dual product architecture require careful content modeling to handle the product categorization logic

---

## 6. Migration Estimates

### Complexity Assessment

| Factor | Rating | Justification |
|--------|--------|---------------|
| Template Count | Very High | 15 distinct templates with complex layouts |
| Component Count | Very High | 48 components, many with high interactive complexity |
| Page Volume | Very High | ~120+ pages including extensive content hub and detail pages |
| Interactive Features | Very High | Quiz engine, product comparison, social engagement (likes/comments), custom can designer |
| Third-Party Integrations | Very High | 16+ integrations including unique ad-tech (DoubleClick, MiQ, Vindico) |
| Content Complexity | Very High | Multi-year content hub, 21 conservation projects, 15 expeditions, 15+ quizzes |
| Authentication/Personalization | Very High | VIA SSO, MFA, personalized coupons, coupon badge, savings tracker |
| Media Complexity | High | Extensive Brightcove video (every Outdoor Corps page), photo carousels, project maps |

### Effort Breakdown

| Phase | Estimated Days | Details |
|-------|---------------|---------|
| **Discovery & Planning** | 10–12 | Template analysis, content audit of ~120+ pages, API documentation review, quiz/social feature scoping |
| **Design System Migration** | 8–10 | Grizzly brand system, dual product category styling (Moist Snuff + Spitfree), dark theme elements, responsive patterns |
| **Global Components** | 10–14 | Header with dynamic coupon badge, footer, health warning with dynamic labels, VIA SSO integration, MFA flow |
| **Content Hub (Grizz List)** | 12–16 | Article templates, social engagement (likes/comments API), category filtering, sequential navigation, multi-year content index |
| **Grizz Quiz Engine** | 14–18 | Multi-step quiz interaction, state management, attempt tracking, result calculation, quiz catalog, category filtering |
| **Product System** | 12–16 | Multi-axis filtering, product comparison widget, flavor profile visualizations, tobacco blend breakdown, Pairs Well With, related products, dual product category (Moist Snuff + Spitfree) |
| **Outdoor Corps** | 10–14 | Project listing, expedition listing, detail templates with video, carousels, maps, related content grids (36 detail pages) |
| **Coupon System** | 8–12 | Personalized dashboard, mail/mobile tabs, savings tracker, Brand API integration, navigation badge |
| **Store Locator** | 6–8 | Google Maps integration, zip code search, geolocation, product filtering, dual product category locators |
| **SMS & Contact** | 4–6 | SMS signup with TCPA compliance, Contact Us (chat/email/call), live chat widget integration |
| **Utility Pages** | 4–6 | FAQ accordion, legal pages, 404 page, My Profile (post-MFA), Custom Cans scope TBD |
| **Content Migration** | 10–14 | ~120+ pages, 21 project detail pages, 15 expedition pages, 15+ articles, 15+ quizzes, 20 product pages |
| **Integration & Testing** | 8–12 | Adobe Analytics, Brightcove, Google Maps, DoubleClick/Floodlight, Brand API, end-to-end testing |
| **QA & Performance** | 6–8 | Cross-browser testing, mobile responsiveness, accessibility audit, performance optimization, Lighthouse scoring |
| **TOTAL** | **120–180** | **person-days** |

### Risk Factors

1. **Grizz Quiz Engine:** The interactive quiz with server-side attempt tracking is the highest-complexity custom feature. May require a dedicated JS application within EDS blocks.
2. **Social Engagement Layer:** Likes and comments on Grizz List articles require backend API services that may not be part of the standard Brand API.
3. **Custom Can Designer:** This feature behind MFA was not fully analyzable. If it involves canvas-based image manipulation, it adds significant development scope.
4. **Ad-Tech Integration Complexity:** DoubleClick/Floodlight, MiQ Digital, and Vindico Suite are unique to mygrizzly.com and require specific tracking pixel/script migration.
5. **Content Volume:** With ~120+ pages including actively growing content hubs (new quizzes and articles being added), content migration requires automated tooling.
6. **Dynamic Warning Labels:** The context-dependent health warning system (MOIST SNUFF / SNUS / Moist Snuff and Snus) needs a content-driven solution.

### Migration Recommendation

**mygrizzly.com should be one of the LAST RAI brands migrated**, given its exceptional complexity. It has the highest page count, most interactive features, and deepest content engagement platform of any RAI brand analyzed. The Grizz Quiz, Grizz List social engagement, product comparison, and Outdoor Corps programs all require custom development beyond standard EDS block patterns.

**Recommended pilot candidates for EDS migration (in order):**
1. **kodiakisking.com** (~11 pages, simplest RAI site)
2. **grizzlynicotinepouches.com** (~15 pages, simple product focus)
3. **cougardips.com** (~20 pages, straightforward structure)
4. **luckystrike.com** (~25 pages, limited features)

Once patterns are established from simpler brands, the mygrizzly.com migration can leverage those reusable components (VIA SSO, Brand API, header/footer, store locator) while focusing custom development on its unique interactive features.

---

*Report generated by Adobe Professional Services — March 31, 2026*
