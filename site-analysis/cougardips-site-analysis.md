# CougarDips.com - Comprehensive Site Analysis

**Prepared for:** Adobe Edge Delivery Services Migration Assessment
**Date:** March 31, 2026
**Analyst:** Adobe Experience Catalyst
**URL:** https://www.cougardips.com/
**Brand Owner:** American Snuff Company, LLC (subsidiary of Reynolds American Inc. / BAT)
**Product Category:** Moist Smokeless Tobacco (Snuff/Dip)

---

## Executive Summary

CougarDips.com is a consumer-facing brand website for Cougar moist smokeless tobacco products, operated by American Snuff Company under the RAI Services umbrella. The site is built on **Adobe Experience Manager (AEM) as a Cloud Service** and follows the same shared RAI platform architecture as other Reynolds American brand sites (americanspirit.com, camel.com, camelsnus.com, vusevapor.com).

Compared to other RAI brand sites, CougarDips.com is notably **simpler and more compact**, with approximately 15-20 unique pages, 6 product SKUs, and a focused feature set centered on coupons, store location, and user-generated content promotions. The site does not include a rewards/loyalty program or content hub.

**Key Characteristics:**
- Age-gated (21+) with VIA/SSO cross-brand authentication
- MFA-protected profile management
- Health warning: "WARNING: This product can cause mouth cancer."
- Product label: "MOIST SNUFF"
- Simpler site architecture (~15-20 pages vs 40-55+ for vusevapor.com)
- User-generated content features (Employee of the Month, Show Your Work)
- Personalized coupon delivery (Mail and Mobile)
- No rewards/loyalty program
- No content hub or blog
- Live chat support via Salesforce (bat-us.my.site.com)

---

## 1. Templates Inventory

### Template 1: Homepage
**URL:** `/secure.html`
**Description:** Full-width hero-driven landing page with promotional sections, product imagery, and call-to-action banners. Features a rotating hero area with the current promotion (Employee of the Month), multiple "Cougar Tech Works" promotional sections with different visual treatments, a full-width product image banner, and store locator CTA.

**Layout Structure:**
- Full-width hero banner with promotion (Employee of the Month promo with "Show Your Work" CTA)
- "Cougar Tech Works" section - dark theme with text overlay on image (variant 1)
- "Cougar Tech Works" section - product image with description overlay (variant 2)
- Full-width product lifestyle image banner
- Store Locator CTA banner with "Find Cougar Near You" heading
- Footer with navigation links and health warning

**Key Components:**
- Hero carousel/banner with CTAs
- Promotional content cards (2 variants)
- Full-width image banner
- Store locator CTA module
- Persistent health warning banner ("MOIST SNUFF / WARNING: This product can cause mouth cancer.")
- Hamburger navigation menu (Products, Find A Store, Employee of the Month, Get A Coupon, Profile)

### Template 2: Products Listing
**URL:** `/secure/products.html`
**Description:** Product catalog page displaying all 6 Cougar product variants in an alternating left-right layout. Each product includes a can image, product name, and brief description.

**Products Listed:**
1. Long Cut Wintergreen
2. Long Cut Straight
3. Long Cut Natural
4. Fine Cut Natural
5. Snuff
6. Pouches

**Layout Structure:**
- Page heading "PRODUCTS"
- Alternating product rows (image-left/text-right, then image-right/text-left)
- Each product: can image + product name + description text
- Footer navigation and health warning

### Template 3: Find A Store (Store Locator)
**URL:** `/secure/find-a-store.html`
**Description:** Google Maps-based store locator with zip code search and geolocation support. Allows users to find nearby retailers carrying Cougar products.

**Layout Structure:**
- Page heading "FIND A STORE"
- Search input field (zip code)
- "Use My Location" geolocation button
- Google Maps embed (interactive)
- Results list area
- Footer and health warning

**Key Components:**
- Google Maps API integration
- Zip code search form
- Geolocation (HTML5 Geolocation API)
- Store results list with distance sorting

### Template 4: Employee of the Month (Promotion)
**URL:** `/secure/employee-of-the-month.html`
**Description:** User-generated content promotion page where users can submit photos of their work to win a $1,000 monthly prize. Features a photo upload form, user submission gallery with "Load more" pagination, and link to previous winners.

**Layout Structure:**
- Hero banner with "Employee of the Month" heading and $1,000 prize callout
- Photo upload CTA ("Enter Now" button)
- User submission gallery (grid of uploaded photos with usernames)
- "Load More" button for pagination
- Links to Official Rules, FAQs, Submission Guidelines, and Winners
- Footer and health warning

**Key Components:**
- Photo upload form (UGC submission)
- Image gallery grid with lazy loading
- "Load More" pagination
- Legal links (Official Rules, Guidelines)

### Template 5: Coupons
**URL:** `/secure/coupons.html`
**Description:** Personalized coupon delivery page showing available coupons for the authenticated user. Features Mail/Mobile toggle, step-by-step redemption instructions, and legal terms.

**Layout Structure:**
- "COUPONS" heading with personalized coupon count ("2 coupons available for you!")
- Mail / Mobile toggle tabs
- Coupon display area (personalized to user)
- 4-step redemption instructions with icons:
  1. Find a participating store
  2. Buy any qualifying product
  3. Upload receipt
  4. Wait for redemption
- Legal terms and conditions
- Footer and health warning

**Key Components:**
- Personalized coupon display (API-driven)
- Mail/Mobile delivery toggle
- Step-by-step instruction cards with icons
- Receipt upload functionality
- Terms accordion/text

### Template 6: Show Your Work (UGC Gallery)
**URL:** `/secure/show-your-work.html`
**Description:** User-generated content gallery page where users can submit photos and browse other submissions. Similar to Employee of the Month but appears to be a standalone content gallery.

**Layout Structure:**
- Hero section with "Show Your Work" branding
- Photo upload CTA
- User submission gallery (grid layout)
- "Load More" button for pagination
- Footer and health warning

**Key Components:**
- Photo upload/submission form
- Image gallery grid
- Lazy loading with "Load More"
- User attribution (usernames)

### Template 7: Winners
**URL:** `/secure/promotions/employee-of-the-month/winners.html`
**Description:** Historical winners page displaying monthly Employee of the Month winners from the program's inception. Each winner entry includes photo, name/description, location, and date.

**Layout Structure:**
- "WINNERS" heading
- Chronological list of monthly winners (newest first)
- Each winner card: photo, name, description, city/state, month/year
- Winners listed from February 2026 back to July 2024
- Footer and health warning

**Key Components:**
- Winner profile cards with images
- Date-based chronological ordering
- Location display (city, state)

### Template 8: FAQ (General)
**URL:** `/secure/footer-links/faq.html`
**Description:** Accordion-based FAQ page organized by topic categories. Categories include Offers & Promotions, Age Verification, Privacy, Troubleshooting, and General.

**Layout Structure:**
- "FAQ" heading
- Accordion sections by category:
  - Offers & Promotions
  - Age Verification
  - Privacy
  - Troubleshooting
  - General
- Each section expands to reveal Q&A pairs
- Footer navigation and health warning

**Key Components:**
- Accordion/collapsible sections (AEM Core Component - likely Accordion)
- Category-based organization
- Nested Q&A pairs within each category

### Template 9: FAQ (Promotion-Specific)
**URL:** `/secure/promotions/employee-of-the-month/faqs.html`
**Description:** Promotion-specific FAQ page for the Employee of the Month program. Features Q&A format with structured content including a judging period table showing monthly submission and judging dates.

**Layout Structure:**
- Promotion-specific FAQ heading
- Q&A pairs related to the promotion
- Judging period table (month-by-month schedule)
- Links back to promotion page
- Footer and health warning

### Template 10: Contact Us
**URL:** `/secure/footer-links/contact-us.html`
**Description:** Multi-channel contact page with Chat, Email, and Call options. Features a live chat button (Salesforce-powered), email contact form with topic dropdown, and phone number.

**Layout Structure:**
- "CONTACT US" heading
- Hours of operation (Mon-Fri 8:00 AM - 10:00 PM ET, Sat 10:00 AM - 8:00 PM ET)
- Three contact channels:
  1. **Chat** - Live chat button (Salesforce integration)
  2. **Email** - Topic dropdown + message textarea + submit button
  3. **Call** - Phone number button (1-866-843-0636)
- Footer navigation and health warning

**Key Components:**
- Salesforce Live Chat integration (bat-us.my.site.com/ESWLiveChatCougar)
- Email form with topic categorization (General, Product Related, Website Issue, Promotion, Technical Help, Coupons, Others)
- Click-to-call phone button

### Template 11: Legal/Policy Pages
**URLs:**
- `/secure/footer-links/terms-of-use.html` - Terms and Conditions of Use
- `/secure/footer-links/privacy-policy.html` - Privacy Policy and State Privacy Rights
- `/secure/footer-links/site-requirements.html` - Site/Browser Requirements

**Description:** Standard legal and policy pages with long-form text content, table of contents with anchor links, and "Back to Top" navigation. Terms of Use includes 15 sections covering age restrictions, account management, dispute resolution, etc.

**Layout Structure:**
- Page heading
- Table of contents with anchor links (Terms of Use)
- Long-form text content with section headings
- "Back to Top" links between sections
- Footer navigation and health warning

### Template 12: My Profile (MFA-Protected)
**URL:** `/secure/my-profile.html`
**Description:** User profile management page behind multi-factor authentication. Requires a one-time passcode sent to the user's email. Full profile page not accessible without MFA completion.

**Layout Structure:**
- MFA verification overlay:
  - "Enter Passcode" heading
  - Email display (masked)
  - Passcode input field
  - "Continue" button
  - Help text about passcode delay
- State selection dropdown (visible behind overlay)
- Profile form (behind MFA gate)

### Template 13: 404 Error Page
**URL:** Any non-existent path
**Description:** Custom 404 page with brand-appropriate messaging ("WELL, CRAP.") and redirect link to homepage.

**Layout Structure:**
- "WELL, CRAP." heading
- Descriptive text with homepage link
- Full footer navigation with all page links
- Health warning banner

### Template 14: Age Gate / Login
**URL:** `/` (root, pre-authentication)
**Description:** Age verification and authentication page. All visitors must verify 21+ age and authenticate before accessing site content. Uses VIA/SSO shared across RAI brand sites.

**Layout Structure:**
- Brand logo
- Login form (email + password)
- Age verification
- Registration link
- Cross-brand SSO integration

---

## 2. Blocks / Components Catalog

### Navigation & Chrome Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 1 | **Header / Navigation Bar** | Fixed header with Cougar logo (left), hamburger menu (right). Menu expands to show: Products, Find A Store, Employee of the Month, Get A Coupon, Profile | All pages | Medium |
| 2 | **Hamburger Menu** | Mobile-first slide-out navigation menu with page links | All pages | Medium |
| 3 | **Footer Navigation** | Two-row footer: Row 1 = main nav (Home, Products, Find A Store, Show Your Work, Get A Coupon, My Profile, Logout); Row 2 = legal links (Contact Us, FAQ, Tobacco Rights, Site Requirements, Terms of Use, Privacy Policy) | All pages | Low |
| 4 | **Health Warning Banner** | Persistent bottom banner: "MOIST SNUFF" label + "WARNING: This product can cause mouth cancer." Full-width, high-contrast styling | All pages | Low |

### Hero & Promotional Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 5 | **Hero Banner** | Full-width hero with background image, heading text, description, and CTA button. Used for main promotional messaging | Homepage | Medium |
| 6 | **Promotional Card - Dark Theme** | Dark background promotional section with heading, descriptive text, and CTA. "Cougar Tech Works" variant with $10,000 prize callout | Homepage | Medium |
| 7 | **Promotional Card - Image Overlay** | Product/lifestyle image with text overlay and CTA. Second "Cougar Tech Works" variant | Homepage | Medium |
| 8 | **Full-Width Image Banner** | Edge-to-edge lifestyle/product photography banner. No text overlay | Homepage | Low |
| 9 | **Store Locator CTA** | Branded banner with "Find Cougar Near You" heading and "Find A Store" button | Homepage | Low |

### Product Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 10 | **Product Card - Left Image** | Product can image on left, product name and description on right. Alternating layout pattern | Products page (3 items) | Low |
| 11 | **Product Card - Right Image** | Product can image on right, product name and description on left. Alternating layout pattern | Products page (3 items) | Low |

### Interactive / Functional Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 12 | **Store Locator Map** | Google Maps integration with zip code search, geolocation, and store results. Uses Google Maps JavaScript API | Find A Store | High |
| 13 | **Photo Upload Form** | User-generated content submission form for uploading photos. Used for Employee of the Month and Show Your Work promotions | Employee of Month, Show Your Work | High |
| 14 | **Image Gallery Grid** | Grid layout displaying user-submitted photos with usernames. Supports lazy loading via "Load More" button | Employee of Month, Show Your Work | Medium |
| 15 | **Load More Button** | Pagination control for loading additional gallery content | Employee of Month, Show Your Work, Winners | Low |
| 16 | **Winner Profile Card** | Card displaying monthly winner photo, name, description, location (city/state), and date | Winners page | Low |

### Coupon Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 17 | **Personalized Coupon Display** | API-driven coupon display showing available coupons for authenticated user. Shows count and coupon details | Coupons | High |
| 18 | **Mail/Mobile Toggle** | Tab-style toggle switch between Mail and Mobile coupon delivery methods | Coupons | Medium |
| 19 | **Step-by-Step Instructions** | 4-step visual instruction block with numbered icons and descriptions for coupon redemption | Coupons | Low |

### Form & Contact Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 20 | **Contact Form** | Email contact form with topic dropdown (8 categories), message textarea, and submit button | Contact Us | Medium |
| 21 | **Live Chat Widget** | Salesforce-powered live chat button and widget (bat-us.my.site.com/ESWLiveChatCougar). Floating chat bubble on some pages | Contact Us, floating | High |
| 22 | **Click-to-Call Button** | Styled phone number button (1-866-843-0636) | Contact Us | Low |

### Content & Legal Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 23 | **Accordion / Collapsible Section** | Expandable content sections organized by category. AEM Core Component (Tabs component referenced in console) | FAQ | Medium |
| 24 | **Table of Contents (Anchor Links)** | In-page navigation with anchor links to sections. "Back to Top" links between sections | Terms of Use | Low |
| 25 | **Long-Form Text Content** | Structured legal/policy text with headings, paragraphs, lists, and inline links | Terms, Privacy, Site Reqs | Low |
| 26 | **Judging Period Table** | Structured HTML table showing monthly submission and judging date ranges | Employee of Month FAQs | Low |

### Authentication Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 27 | **Age Gate / Login Form** | VIA/SSO age verification and login. Email + password fields with "Remember Me" option | Login page | High |
| 28 | **MFA Passcode Form** | One-time passcode verification overlay. Displays target email, passcode input, continue button | My Profile | High |

### Utility Components

| # | Component | Description | Instances | Complexity |
|---|-----------|-------------|-----------|------------|
| 29 | **404 Error Page** | Custom "WELL, CRAP." error message with homepage redirect link and full footer | Error pages | Low |
| 30 | **Service Worker Cache** | Background caching via `resource-cache-service-worker.js` with `cougar-cache-config.json` | Site-wide | Medium |

**Total Unique Components: 30**

---

## 3. Page Counts by Template

| Template | Estimated Page Count | Example URLs |
|----------|---------------------|--------------|
| Homepage | 1 | `/secure.html` |
| Products Listing | 1 | `/secure/products.html` |
| Find A Store | 1 | `/secure/find-a-store.html` |
| Employee of the Month | 1 | `/secure/employee-of-the-month.html` |
| Coupons | 1 | `/secure/coupons.html` |
| Show Your Work | 1 | `/secure/show-your-work.html` |
| Winners | 1 | `/secure/promotions/employee-of-the-month/winners.html` |
| FAQ (General) | 1 | `/secure/footer-links/faq.html` |
| FAQ (Promotion) | 1 | `/secure/promotions/employee-of-the-month/faqs.html` |
| Contact Us | 1 | `/secure/footer-links/contact-us.html` |
| Legal/Policy | 3 | Terms of Use, Privacy Policy, Site Requirements |
| My Profile | 1 | `/secure/my-profile.html` |
| 404 Error | 1 | Any non-existent URL |
| Age Gate / Login | 1 | `/` (root) |
| Promotion Pages (Seasonal) | ~2-3 | Cougar Tech Works, Official Rules, Submission Guidelines |
| **TOTAL** | **~18-20** | |

**Notes:**
- CougarDips.com is the simplest site in the RAI portfolio analyzed
- No individual product detail pages (products shown only in listing)
- No content hub, blog, or editorial content
- Seasonal promotions may add/remove pages (Cougar Tech Works returned 404)
- Tobacco Rights link redirects externally to ownitvoiceit.com (RAI advocacy site)

---

## 4. Integrations Analysis

### Adobe Experience Cloud

| Integration | Details | Status |
|-------------|---------|--------|
| **Adobe Experience Platform Launch** | Tag management: `launch-EN66d1505d231e4d7a8fc8c95533aae9b5.min.js` with 60+ extensions | Active |
| **Adobe Analytics** | AppMeasurement v2.22.4, Report Suite: `raiservices.global.prod`, Tracking Server: `raiservices.sc.omtrdc.net` | Active |
| **Adobe Target** | AT.js v2.11.4, Client Code: `raiservices`, View-based triggering (e.g., `secure:employee-of-the-month`) | Active |
| **Adobe Audience Manager** | v9.4, Visitor API for audience segmentation | Active |
| **Adobe Visitor ID Service** | Organization: `02D9C50759DEA0920A495ED3@AdobeOrg`, Cross-brand visitor identification | Active |
| **Adobe Client Data Layer** | v2.0.2, 35+ tracked events on page load, AEM Core Components Data Layer v1 | Active |

### Authentication & Identity

| Integration | Details | Status |
|-------------|---------|--------|
| **VIA/SSO Authentication** | Cross-brand SSO via `securePage()` function, shared login across RAI sites | Active |
| **Multi-Factor Authentication (MFA)** | One-time passcode via email for profile access, prevents unauthorized profile changes | Active |
| **Brand Site API** | REST API at `https://api.cougardips.com`, Site Key: `cougar` | Active |

### Third-Party Services

| Integration | Details | Status |
|-------------|---------|--------|
| **Google Maps API** | Interactive store locator on Find A Store page, JavaScript API with custom markers | Active |
| **Salesforce Live Chat** | Live chat widget via `bat-us.my.site.com/ESWLiveChatCougar`, Pre-chat API detected | Active |
| **DoubleClick (Google)** | Conversion tracking, Floodlight ID: `11201219`, endpoint: `11201219.fls.doubleclick.net` | Active |

### Fonts & Typography

| Integration | Details | Status |
|-------------|---------|--------|
| **Google Fonts** | Fira Sans (weight 900), Saira Semi Condensed (weights 600, 800) | Active |
| **Adobe Typekit** | Custom font kit: `lwx6gwj.css` via `use.typekit.net` | Active |

### Performance & Monitoring

| Integration | Details | Status |
|-------------|---------|--------|
| **Adobe Helix RUM** | Real User Monitoring via `rum.hlx.page` | Active |
| **Service Worker Caching** | `resource-cache-service-worker.js` with `cougar-cache-config.json` for offline/performance | Active |
| **Google Site Verification** | Meta tag: `5kD4bClxtkw8v_qlZLCE7at6_yWWTRw4WO1N4a02VFc` | Active |

### AEM Platform

| Integration | Details | Status |
|-------------|---------|--------|
| **AEM as a Cloud Service** | Adobe Experience Manager cloud platform, Core Components | Active |
| **AEM Core Components** | Tabs, Accordion, and other standard components. Console warnings about `container.utils` not available suggest some components partially configured | Active (with warnings) |

### Integration Count Summary

| Category | Count |
|----------|-------|
| Adobe Experience Cloud | 6 |
| Authentication & Identity | 3 |
| Third-Party Services | 3 |
| Fonts & Typography | 2 |
| Performance & Monitoring | 3 |
| AEM Platform | 2 |
| **Total Integrations** | **19** |

---

## 5. Complex Use Cases & Observations

### 5.1 User-Generated Content (UGC) System

**Complexity: HIGH**

CougarDips.com has a significant UGC component that sets it apart from other RAI brand sites:

- **Employee of the Month Program:** Users submit photos of their work for a chance to win $1,000/month ($12,000/year total). Includes photo upload, moderation workflow, gallery display, voting/selection, and winner announcement.
- **Show Your Work Gallery:** Standalone UGC gallery where users share content. Features upload, gallery grid, lazy loading, and user attribution.
- **Content Moderation:** Implied by Submission Guidelines link and Terms of Use content moderation section. Likely involves backend review workflow before content appears publicly.

**Migration Considerations:**
- UGC upload/submission forms would need custom EDS block development
- Image storage and moderation workflows would require headless API integration
- Gallery grid with lazy loading and "Load More" pagination is a custom interactive component
- Winner selection and announcement workflow may be manual/backend-driven

### 5.2 Personalized Coupon System

**Complexity: HIGH**

The coupon system is personalized per user and integrates with the Brand Site API:

- Coupons are dynamically loaded based on authenticated user profile
- "2 coupons available for you!" - personalized messaging
- Mail/Mobile delivery options suggest integration with a coupon fulfillment system
- 4-step receipt upload and redemption process implies a multi-step workflow
- Legal terms and conditions are coupon-specific

**Migration Considerations:**
- Coupon display requires API integration with the Brand Site API
- Receipt upload functionality needs custom block development
- Personalization based on user profile/location/history
- Mail fulfillment implies physical coupon printing and mailing system

### 5.3 Age Gate and Authentication

**Complexity: HIGH**

Standard RAI cross-brand authentication but with some unique aspects:

- VIA/SSO shared login across all RAI brand sites
- MFA enforcement for profile access (one-time passcode via email)
- `securePage()` JavaScript function enforces authentication on all `/secure/` paths
- State selection visible on profile page suggests geo-specific content/offers
- Session management with API endpoint for login verification

**Migration Considerations:**
- Age gate must be implemented as a pre-rendering check
- SSO integration needs coordination across multiple brand properties
- MFA flow requires email delivery and verification logic
- Profile data likely stored in centralized RAI identity system

### 5.4 Google Maps Store Locator

**Complexity: MEDIUM-HIGH**

- Google Maps JavaScript API with custom styling and markers
- Zip code search with geocoding
- HTML5 Geolocation API ("Use My Location")
- Store data likely fetched from Brand Site API or dedicated service
- Results displayed as list with distance calculations

**Migration Considerations:**
- Google Maps API key management and billing
- Store database/API integration
- Geolocation permission handling
- Custom map styling to match brand design

### 5.5 Salesforce Live Chat Integration

**Complexity: MEDIUM**

- Salesforce Embedded Service Chat via `bat-us.my.site.com/ESWLiveChatCougar`
- Pre-chat API detected in console logs
- Floating chat widget appears on some pages
- Integration with Salesforce Service Cloud for agent routing

**Migration Considerations:**
- Salesforce chat snippet embedding in EDS
- Pre-chat form/API integration
- Chat availability hours management
- Page-specific chat activation rules

### 5.6 Seasonal/Expiring Promotions

**Observation:** The "Cougar Tech Works" promotion linked from the homepage returned a 404 error, indicating it has expired or been removed. However, the homepage still references it with two prominent promotional sections.

**Implication:** Content management must account for promotional lifecycle:
- Promotions have start/end dates
- Homepage content references may outlive promotion pages
- Official Rules, FAQ, and Winners pages associated with promotions need lifecycle management
- Employee of the Month has been running since at least July 2024 (earliest winner shown)

### 5.7 Console Warnings and Technical Debt

**Observed Issues:**
- `TypeError: w[l].push is not a function` - Occurs on every page, suggests a global JavaScript conflict
- `Tabs: container utilities at window.CQ.CoreComponents.container.utils are not available` - AEM Core Components configuration issue
- `Failed to load resource: 404` - Missing resources on some pages
- `Refused to execute script from 'undefined'` - Script source resolution failures on Contact Us page

**Migration Opportunity:** These console errors indicate technical debt that could be resolved during EDS migration, resulting in a cleaner, more performant codebase.

### 5.8 Brand Design Language

**Typography:**
- Primary font: Fira Sans (Google Fonts, weight 900) - used for bold headings
- Secondary font: Saira Semi Condensed (Google Fonts, weights 600, 800) - used for subheadings and accent text
- Adobe Typekit kit (`lwx6gwj.css`) provides additional brand fonts

**Color Palette:**
- Primary: Dark/Black (#000000 or near-black) backgrounds
- Accent: Burnt orange/brown (#C25400 or similar) for CTAs and highlights
- Text: White on dark backgrounds, dark on light backgrounds
- Warning: Black and white high-contrast for health warning banner

**Design Style:**
- Rugged, masculine aesthetic appropriate for moist snuff brand
- Heavy use of dark backgrounds with light text
- Industrial/workwear imagery (aligned with "Employee of the Month" working theme)
- Compact layout with minimal whitespace

---

## 6. Migration Estimates

### Effort Breakdown by Category

#### A. Design System & Global Styles
| Task | Effort (Person-Days) |
|------|---------------------|
| Design token extraction (colors, typography, spacing) | 2 |
| Global CSS variables and responsive framework | 2 |
| Font integration (Google Fonts + Typekit) | 0.5 |
| Health warning banner component | 0.5 |
| **Subtotal** | **5** |

#### B. Navigation & Chrome
| Task | Effort (Person-Days) |
|------|---------------------|
| Header with logo and hamburger menu | 2 |
| Mobile navigation slide-out | 1.5 |
| Footer (two-row navigation) | 1 |
| **Subtotal** | **4.5** |

#### C. Page Templates
| Task | Effort (Person-Days) |
|------|---------------------|
| Homepage layout | 2 |
| Products listing (alternating layout) | 1.5 |
| Find A Store page | 1 |
| Employee of the Month / Show Your Work | 2 |
| Coupons page | 1.5 |
| Winners page | 1 |
| FAQ pages (2 variants) | 1 |
| Contact Us page | 1 |
| Legal/Policy template | 0.5 |
| Profile page | 1 |
| 404 Error page | 0.5 |
| Age Gate / Login | 1 |
| **Subtotal** | **14** |

#### D. Block Development
| Task | Effort (Person-Days) |
|------|---------------------|
| Hero banner block | 2 |
| Promotional card blocks (2 variants) | 2 |
| Product card block (alternating layout) | 2 |
| Image gallery grid with Load More | 3 |
| Photo upload/submission form | 3 |
| Winner profile card | 1 |
| Accordion/FAQ block | 1.5 |
| Step-by-step instructions block | 1 |
| Mail/Mobile toggle | 1 |
| Contact form block | 1.5 |
| Table of contents block | 1 |
| Store locator CTA block | 0.5 |
| Full-width image banner | 0.5 |
| **Subtotal** | **20** |

#### E. Integrations
| Task | Effort (Person-Days) |
|------|---------------------|
| Age gate/VIA SSO authentication | 5 |
| MFA implementation | 3 |
| Brand Site API integration | 3 |
| Personalized coupon system | 5 |
| Google Maps store locator | 3 |
| Salesforce Live Chat | 2 |
| Adobe Analytics/Launch migration | 3 |
| Adobe Target migration | 2 |
| DoubleClick conversion tracking | 1 |
| Service Worker / caching strategy | 1 |
| **Subtotal** | **28** |

#### F. Content Migration
| Task | Effort (Person-Days) |
|------|---------------------|
| Content authoring for ~18-20 pages | 3 |
| Image asset migration and optimization | 1 |
| Legal content migration (3 pages) | 1 |
| FAQ content migration | 0.5 |
| Product content migration | 0.5 |
| **Subtotal** | **6** |

#### G. Testing & QA
| Task | Effort (Person-Days) |
|------|---------------------|
| Cross-browser testing | 2 |
| Mobile responsive testing | 2 |
| Accessibility audit (WCAG 2.1 AA) | 2 |
| Performance optimization (Core Web Vitals) | 2 |
| Integration testing (auth, coupons, maps) | 3 |
| UAT support | 2 |
| **Subtotal** | **13** |

### Summary

| Category | Low Estimate | High Estimate |
|----------|-------------|---------------|
| Design System & Global Styles | 4 | 6 |
| Navigation & Chrome | 4 | 6 |
| Page Templates | 12 | 16 |
| Block Development | 17 | 24 |
| Integrations | 24 | 34 |
| Content Migration | 5 | 8 |
| Testing & QA | 11 | 16 |
| **TOTAL** | **77** | **110** |

### Risk-Adjusted Estimate

| Scenario | Person-Days | Calendar Weeks (2-person team) |
|----------|-------------|-------------------------------|
| **Optimistic** (minimal scope changes, smooth integrations) | 77 | 8-9 weeks |
| **Most Likely** (standard scope, moderate integration complexity) | 90 | 9-10 weeks |
| **Pessimistic** (scope additions, integration challenges, UGC complexity) | 110 | 11-12 weeks |

### Key Risk Factors

1. **UGC System Complexity:** Photo upload, moderation, and gallery display may require more custom development than estimated if the existing backend API is not well-documented
2. **Coupon Personalization:** Deep integration with coupon fulfillment system; receipt upload workflow may have undocumented requirements
3. **Authentication/SSO:** Cross-brand SSO coordination involves multiple stakeholders and may have dependencies on other brand site timelines
4. **Seasonal Content Lifecycle:** Promotional content management (Employee of the Month, Cougar Tech Works) needs a clear lifecycle strategy
5. **Salesforce Chat:** Integration complexity depends on Salesforce configuration and may require Salesforce admin involvement

### Comparison to Other RAI Brand Sites

| Site | Pages | Components | Integrations | Estimated Days |
|------|-------|------------|-------------|---------------|
| americanspirit.com | ~25-30 | ~35 | ~25 | 120-170 |
| camel.com | ~30-40 | ~40 | ~30 | 150-210 |
| camelsnus.com | ~20-25 | ~30 | ~22 | 100-140 |
| vusevapor.com | ~48-55 | ~40 | ~32 | 195-310 |
| **cougardips.com** | **~18-20** | **~30** | **~19** | **77-110** |

CougarDips.com represents the **smallest and least complex** site in the RAI brand portfolio, making it an ideal candidate for a pilot migration or early phase of a multi-brand EDS migration program.

---

## Appendix: Screenshots

### Screenshot 1: Homepage
![Homepage](/workspace/site-analysis/screenshots/cougar-01-homepage.png)

### Screenshot 2: Products
![Products](/workspace/site-analysis/screenshots/cougar-02-products.png)

### Screenshot 3: Find A Store
![Find A Store](/workspace/site-analysis/screenshots/cougar-03-find-a-store.png)

### Screenshot 4: Employee of the Month
![Employee of the Month](/workspace/site-analysis/screenshots/cougar-04-employee-of-month.png)

### Screenshot 5: Coupons
![Coupons](/workspace/site-analysis/screenshots/cougar-05-coupons.png)

### Screenshot 6: Show Your Work
![Show Your Work](/workspace/site-analysis/screenshots/cougar-06-show-your-work.png)

### Screenshot 7: Winners
![Winners](/workspace/site-analysis/screenshots/cougar-07-winners.png)

### Screenshot 8: FAQ
![FAQ](/workspace/site-analysis/screenshots/cougar-08-faq.png)

### Screenshot 9: Contact Us
![Contact Us](/workspace/site-analysis/screenshots/cougar-09-contact-us.png)

### Screenshot 10: Profile (MFA Gate)
![Profile MFA](/workspace/site-analysis/screenshots/cougar-10-profile-mfa.png)
