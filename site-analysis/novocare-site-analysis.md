# NovoCare (novocare.com) — Comprehensive Site Analysis

**Prepared for:** Adobe Experience Manager Edge Delivery Services Migration Assessment
**Analysis Date:** April 2, 2026
**Analyst:** Adobe Professional Services

---

## Executive Summary

NovoCare (novocare.com) is the patient support portal for **Novo Nordisk**, a global pharmaceutical company specializing in diabetes, obesity, and other chronic conditions. The site is built on **Adobe Experience Manager (AEM) as a Cloud Service** using the `brandbase-novocare-page-template` template framework with extensive custom client libraries.

NovoCare serves as a **savings, coverage, and support hub** for patients prescribed Novo Nordisk medications across 7 therapeutic areas: Diabetes, Obesity/Weight Loss, MASH (metabolic dysfunction-associated steatohepatitis), Growth-Related Disorders, Hemophilia and Bleeding Disorders, Primary Hyperoxaluria Type 1 (PH1), and Women's Health. The site also includes a parallel HCP (Health Care Professional) experience and a dedicated NovoCare Pharmacy section.

**Key Metrics:**
- **Total Pages (from sitemap):** 214
- **Templates Identified:** 10
- **Components/Blocks Cataloged:** 28
- **Third-Party Integrations:** 12+
- **Therapeutic Areas:** 7 (patient) + 6 (HCP)
- **Products Covered:** 20+ branded medications
- **Migration Complexity:** High
- **Estimated Migration Effort:** 85–130 person-days

---

## 1. Templates Inventory

### Template 1: Global Homepage

| Field | Detail |
|-------|--------|
| **Template Name** | Global Homepage |
| **Complexity** | Medium |
| **Reasoning** | Condition selector dropdown, promotional cards, pharmacy promo section, dual CTA layout |
| **Reference URL** | https://www.novocare.com/ |

**Description:** Main entry point with hero section featuring H1 "Support starts here", condition selector dropdown (7 conditions), NovoCare Pharmacy promotional card with image, insulin cost savings CTA with icon, and HCP promotional card. Uses a simplified header with therapeutic area links (Diabetes, Weight Loss, MASH, Growth-Related Disorders, Hemophilia, PH1).

![Homepage](screenshots/novocare-01-homepage-clean.png)

### Template 2: Therapeutic Area Home (Multi-Product)

| Field | Detail |
|-------|--------|
| **Template Name** | Therapeutic Area Home — Multi-Product |
| **Complexity** | High |
| **Reasoning** | Full sub-navigation, hero with CTA, icon-based feature cards, image + text section, ISI panels, product-specific content |
| **Reference URLs** | https://www.novocare.com/diabetes/home.html, https://www.novocare.com/growth-related-disorders/home.html, https://www.novocare.com/bleeding-disorders/home.html |

**Description:** Disease-area landing pages with branded sub-navigation tabs (Home, Products, Savings, Insurance, Resources), hero section with H1 and CTA, feature cards with icons (e.g., "Find help with insulin costs", "Check your insurance coverage"), image + text education section, and one or more ISI (Important Safety Information) panels at the bottom. Used for therapeutic areas with multiple products.

![Diabetes Home](screenshots/novocare-02-diabetes-home.png)

### Template 3: Therapeutic Area Home (Single-Product / Branded)

| Field | Detail |
|-------|--------|
| **Template Name** | Therapeutic Area Home — Single-Product Branded |
| **Complexity** | Very High |
| **Reasoning** | Dual-branded header (NovoCare + product logo), numbered step-by-step program walkthrough (up to 7 steps), tabbed insurance process section, savings card promo, multiple ISI panels |
| **Reference URLs** | https://www.novocare.com/mash/home.html, https://www.novocare.com/ph1/home.html |

**Description:** Product-focused landing pages with dual branding (NovoCare logo + product logo like Wegovy or Rivfloza), sub-navigation, hero with enrollment CTA, numbered step-by-step program walkthrough (e.g., 01-Enrollment through 07-Savings offer), tabbed insurance process section (How it works / If approved / If denied), savings card promotion, JumpStart/PAP assistance sections, and full ISI panel. PH1 page includes 6 numbered program steps with device training.

![MASH Home](screenshots/novocare-07-mash.png)

![PH1 Home](screenshots/novocare-09-ph1.png)

### Template 4: Weight Loss / Obesity Home

| Field | Detail |
|-------|--------|
| **Template Name** | Weight Loss Home (Patient Portal) |
| **Complexity** | Very High |
| **Reasoning** | Unique hamburger menu layout (not tab-based), medicine selector combobox, promotional product cards (Wegovy pill), Find a Doctor section, dual ISI panels (Wegovy + Saxenda), compounded semaglutide safety notice |
| **Reference URL** | https://www.novocare.com/patient/home.html (redirected from /obesity.html) |

**Description:** Distinct template from other therapeutic areas. Uses hamburger MENU button instead of tab navigation, "Weight Loss" label, medicine selector combobox ("Choose your medicine"), Wegovy pill promotional card, Find a Doctor section with image cards, pharmacy delivery CTA, and dual ISI panels for Wegovy and Saxenda. Includes a safety notice about compounded semaglutide vs FDA-approved products.

![Obesity Home](screenshots/novocare-03-obesity.png)

### Template 5: HCP Hub

| Field | Detail |
|-------|--------|
| **Template Name** | HCP Portal Hub |
| **Complexity** | Low |
| **Reasoning** | Simple card grid layout, no ISI, minimal components |
| **Reference URL** | https://www.novocare.com/hcp.html |

**Description:** Healthcare Professional landing page with hero section, descriptive text, and 6 therapeutic area cards in a 2-column grid layout (Diabetes, Obesity, MASH, Growth-Related Disorders, Hemophilia, PH1). Each card has an "Explore" CTA. Simplified header with "Support for patients" link. No ISI panels.

![HCP Hub](screenshots/novocare-04-hcp.png)

### Template 6: Pharmacy Landing

| Field | Detail |
|-------|--------|
| **Template Name** | NovoCare Pharmacy Landing |
| **Complexity** | High |
| **Reasoning** | Dedicated pharmacy nav tabs (Pharmacy, Wegovy, Ozempic, Find a Doctor), product pricing, comparison table, FAQ accordion, step-by-step delivery process |
| **Reference URL** | https://www.novocare.com/pharmacy.html |

**Description:** Standalone pharmacy experience with its own navigation tabs, hero with pricing headline ("Get a GLP-1 for as low as $149"), product comparison/pricing table, delivery/pickup steps walkthrough, FAQ accordion, and support CTA. Includes semaglutide safety notice and CoAssist Pharmacy d/b/a NovoCare Pharmacy footnote.

![Pharmacy](screenshots/novocare-05-pharmacy.png)

### Template 7: Content Sub-Page (Cards Layout)

| Field | Detail |
|-------|--------|
| **Template Name** | Content Sub-Page — Card Grid |
| **Complexity** | Medium |
| **Reasoning** | Reusable card-based content layout with icon + text + CTA pattern, grouped by category |
| **Reference URLs** | https://www.novocare.com/diabetes/help-with-costs/help-with-insulin-costs.html, https://www.novocare.com/diabetes/insurance-information/check-coverage.html |

**Description:** Sub-pages within therapeutic areas featuring H1 heading, descriptive text, and grouped card sections. Cards contain icons, descriptions, and CTA links. Used for "Help with costs" (program cards grouped by insurance status) and "Check coverage" (product-by-product coverage check cards). Check coverage pages include full ISI panels for all listed products.

![Insulin Costs](screenshots/novocare-11-insulin-costs.png)

![Check Coverage](screenshots/novocare-12-check-coverage.png)

### Template 8: Contact Us

| Field | Detail |
|-------|--------|
| **Template Name** | Contact Us / Utility Page |
| **Complexity** | Low |
| **Reasoning** | Simple informational layout with contact cards, no complex interactivity |
| **Reference URL** | https://www.novocare.com/contact-us.html |

**Description:** Hero section with H1, 6 therapeutic area contact cards with phone numbers and hours of operation, and a "Report a side effect" section linking to Novo Nordisk's global reporting system. No ISI panels.

![Contact Us](screenshots/novocare-06-contact.png)

### Template 9: Eligibility / Forms Page

| Field | Detail |
|-------|--------|
| **Template Name** | Eligibility & Enrollment Form |
| **Complexity** | High |
| **Reasoning** | Interactive forms with validation, eligibility logic, multi-step enrollment, external form integrations |
| **Reference URLs** | https://www.novocare.com/eligibility/myinsulinrx.html, https://www.novocare.com/eligibility/wegovy-savings-card.html, https://www.novocare.com/eligibility/diabetes-savings-card.html |

**Description:** Form-based pages for savings card enrollment, patient assistance program applications, and pharmacy eligibility. Contains multi-step forms with validation, eligibility criteria checks, and terms acceptance. 16+ eligibility form pages across all therapeutic areas.

### Template 10: Insurance Information (Exploring Insurance)

| Field | Detail |
|-------|--------|
| **Template Name** | Insurance Education Pages |
| **Complexity** | Low–Medium |
| **Reasoning** | Templated informational content, repeated across 5+ therapeutic areas with identical structure |
| **Reference URLs** | https://www.novocare.com/diabetes/insurance-information/exploring-insurance/about.html, https://www.novocare.com/diabetes/insurance-information/insurance-types/commercial.html |

**Description:** Educational content about insurance — repeated across diabetes, obesity, growth-related disorders, bleeding disorders, and PH1. Six "Exploring Insurance" pages (About, Choose a Plan, Terms, FAQ, Tips, Resources) and four "Insurance Types" pages (Commercial, Medicare, Medicaid, Uninsured). Nearly identical structure across all therapeutic areas (~50 pages total).

---

## 2. Blocks / Components Catalog

### Global Components

| # | Block Name | Complexity | Description | Reference URL(s) |
|---|-----------|------------|-------------|-------------------|
| 1 | **Global Header (Patient)** | Medium | Novo Nordisk logo, NovoCare branded logo with "Savings \| Coverage \| Support" tagline, "Support for Health Care Professionals" link. Varies slightly by section — homepage shows therapeutic area links, disease pages show disease label + sub-nav | All patient pages |
| 2 | **Global Header (HCP)** | Low | Similar to patient header but with "For Health Care Professionals" label and "Support for patients" link back to patient site | https://www.novocare.com/hcp.html |
| 3 | **Sub-Navigation Tabs** | Medium | Horizontal tab navigation below header, disease-area specific (e.g., Home, Products, Help with costs, Insurance information, Resources). Active tab highlighted. With dropdown menus on some tabs | All therapeutic area pages |
| 4 | **Global Footer** | Medium | Footer links (Terms of Use, Privacy Notice, Consumer Health Privacy Notice, Cookie Notice, Cookie Settings, Your Privacy Choices, Contact Us, Novo Nordisk US), trademark text with registered symbols, copyright notice, Novo Nordisk logo | All pages |
| 5 | **Cookie Consent Banner (OneTrust)** | Low | OneTrust cookie banner with "Customize Cookies", "Reject All", "Accept All Cookies" buttons, privacy notice text | All pages (first visit) |
| 6 | **ISI Panel (Important Safety Information)** | High | Expandable/collapsible safety information panel with "Skip to main content" link, structured headings (What is X?, Who should not take X?, Side effects, etc.), bold warnings, bulleted lists, PI and Medication Guide links, FDA reporting. Multiple ISI panels can stack on a single page | All product-related pages |
| 7 | **ISI Scroll FAB Button** | Low | Floating action button ("Scroll Fab Button") for navigating within ISI content | Pages with ISI panels |

### Hero Components

| # | Block Name | Complexity | Description | Reference URL(s) |
|---|-----------|------------|-------------|-------------------|
| 8 | **Hero — Text + Image** | Medium | Full-width hero with H1 heading, descriptive paragraph, CTA button, and right-aligned photograph. Used on homepage, disease area homes, and HCP hub | https://www.novocare.com/, https://www.novocare.com/hcp.html |
| 9 | **Hero — Text Only** | Low | Simple hero with H1 heading and descriptive text, no image. Used on sub-pages | https://www.novocare.com/diabetes/help-with-costs/help-with-insulin-costs.html |
| 10 | **Hero — Condition Selector** | High | Hero with condition dropdown combobox (7 options), submit arrow button, descriptive text. Redirects to selected therapeutic area | https://www.novocare.com/ |
| 11 | **Hero — Medicine Selector** | High | Hero with "Choose your medicine" combobox for weight loss products, different layout from condition selector | https://www.novocare.com/patient/home.html |
| 12 | **Promotional Banner** | Low | Full-width colored banner with linked text and arrow icon (e.g., "Get FDA-approved GLP-1 RAs shipped directly to your home") | https://www.novocare.com/ |

### Content Cards & Sections

| # | Block Name | Complexity | Description | Reference URL(s) |
|---|-----------|------------|-------------|-------------------|
| 13 | **Feature Card — Icon + Text + CTA** | Medium | Card with SVG icon, uppercase label, heading, description text, and styled CTA button. Used in 2-column grid layouts. Multiple design variants (blue border, pink background, etc.) | https://www.novocare.com/diabetes/home.html |
| 14 | **Feature Card — Image + Text Overlay** | Medium | Card with background image, overlaid text content, heading, and CTA. Used for promotional content like "Find a Doctor" and "Your medicine, delivered" | https://www.novocare.com/patient/home.html |
| 15 | **Product Card** | Medium | Product selection card with product logo/name, brief description, CTA links for "Find out more", ISI link, and PI link | https://www.novocare.com/growth-related-disorders/home.html |
| 16 | **Pharmacy Promo Card** | Medium | Image + text card with NovoCare Pharmacy branding, heading, CTA link, and footnote about CoAssist Pharmacy | https://www.novocare.com/ |
| 17 | **Therapeutic Area Card (HCP)** | Low | Simple text card with therapeutic area name and "Explore" CTA link, used in 2-column grid on HCP hub | https://www.novocare.com/hcp.html |
| 18 | **Contact Card** | Low | Card with therapeutic area name, phone number, and hours of operation | https://www.novocare.com/contact-us.html |
| 19 | **Image + Text Section** | Medium | Two-column layout with illustration/image on one side and heading + text + CTA on the other. Used for education sections and promotional content | https://www.novocare.com/diabetes/home.html |
| 20 | **Savings Card Promotion** | Medium | Styled promotional block showing savings offer details (e.g., "$0 per fill", "$15K annual cap"), eligibility info, and CTA | https://www.novocare.com/ph1/home.html |

### Interactive Components

| # | Block Name | Complexity | Description | Reference URL(s) |
|---|-----------|------------|-------------|-------------------|
| 21 | **Numbered Step-by-Step Walkthrough** | High | Numbered program steps (01-07) showing enrollment process flow. Each step has a number, title, and brief description. Visual progression indicator | https://www.novocare.com/mash/home.html, https://www.novocare.com/ph1/home.html |
| 22 | **Tabbed Insurance Process** | High | Three-tab interface showing "How it works", "If approved", "If denied" insurance process flows. Tab switching reveals different content panels | https://www.novocare.com/ph1/home.html, https://www.novocare.com/bleeding-disorders/home.html |
| 23 | **FAQ Accordion** | Medium | Expandable/collapsible Q&A sections with toggle icons | https://www.novocare.com/pharmacy.html |
| 24 | **Product Coverage Check Card** | Medium | Per-product card with product name, "Check your coverage" CTA linking to product-specific coverage tool | https://www.novocare.com/diabetes/insurance-information/check-coverage.html |
| 25 | **Eligibility Form** | Very High | Multi-step enrollment forms with field validation, eligibility logic, terms acceptance, and integration with external enrollment systems (novocare.iassist.com) | https://www.novocare.com/eligibility/myinsulinrx.html |

### Utility Components

| # | Block Name | Complexity | Description | Reference URL(s) |
|---|-----------|------------|-------------|-------------------|
| 26 | **Compounded Product Safety Notice** | Low | Alert/notice banner warning about compounded semaglutide vs FDA-approved products, with external link | https://www.novocare.com/patient/home.html |
| 27 | **Trademark/Copyright Block** | Low | Footer section with registered trademark symbols, copyright year, document code | All pages |
| 28 | **External Link Card** | Low | Card linking to external sites (e.g., "Find out more about MASH" linking to mash.wegovy.com, "Diabetes education" linking to diabeteseducation.novocare.com) | Various pages |

---

## 3. Page Counts by Template

| Template | Est. Page Count | Auto-Migrate | Manual Migration | Notes |
|----------|----------------|-------------|-----------------|-------|
| Global Homepage | 1 | No | Yes | Condition selector logic, promotional cards |
| Therapeutic Area Home (Multi-Product) | 3 | No | Yes | Diabetes, Growth Disorders, Bleeding Disorders — each unique |
| Therapeutic Area Home (Single-Product) | 2 | No | Yes | MASH, PH1 — branded with product logos, step-by-step flows |
| Weight Loss Home | 1 | No | Yes | Unique layout with medicine selector, dual ISI |
| HCP Hub + HCP Sub-Pages | 25 | Partial | Partial | Hub is simple; sub-pages mirror patient structure |
| Pharmacy Landing + Sub-Pages | 6 | No | Yes | Pricing, comparison, FAQ, product-specific pharmacy pages |
| Content Sub-Pages (Cards) | ~30 | Partial | Partial | Help with costs, savings offers, product pages — card layouts |
| Contact Us | 1 | Yes | No | Simple informational page |
| Eligibility Forms | 16+ | No | Yes | Complex forms with validation and external integrations |
| Insurance Information (Exploring) | ~50 | Yes | No | Highly templated, identical structure across therapeutic areas |
| Product Detail / Check Coverage | ~30 | Partial | Partial | Product-specific with ISI panels |
| Spanish Content | 7 | Partial | Partial | Bleeding disorders only |
| Resources / Safe Disposal | ~10 | Yes | No | Simple content pages |
| Legacy/Archive Pages | ~5 | Yes | No | Older URLs, likely redirects |
| Subdomain (diabeteseducation) | 20+ | No | Yes | Separate site on diabeteseducation.novocare.com |
| **TOTAL** | **~214** | **~75 (35%)** | **~139 (65%)** | |

---

## 4. Integrations & Third-Party Services Analysis

| # | Integration | Type | Complexity | Description | Reference URL(s) |
|---|------------|------|------------|-------------|-------------------|
| 1 | **Adobe Launch (DTM)** | Embed/Tag Manager | Medium | `assets.adobedtm.com/7090418387d1/3d1fd21ee55f/launch-c5ed7c25a38e.min.js` — Tag management for analytics, targeting, and third-party script orchestration | All pages |
| 2 | **Google Tag Manager (GTM)** | Embed/Tag Manager | Medium | GTM container `GTM-T6JLPPW` — Additional tag management layer running alongside Adobe Launch | All pages |
| 3 | **Google Analytics 4 (GA4)** | Embed/Analytics | Medium | Two GA4 property IDs: `G-F40L5513K4` and `G-WXY74XCGE4` — Dual GA4 tracking (likely patient vs HCP or staging vs production) | All pages |
| 4 | **Bing Ads/UET** | Embed/Advertising | Low | `bat.bing.com/bat.js` and action script `187194726.js` — Microsoft Advertising Universal Event Tracking for conversion tracking | All pages |
| 5 | **OneTrust** | Embed/Privacy | Medium | `cdn.cookielaw.org` — Cookie consent management platform with banner, preference center, and SDK. Handles CCPA/GDPR compliance | All pages |
| 6 | **TwentyCI / di-capt** | Embed/Analytics | Low | `cdn.di-capt.com/evaluation/inc.js` — Digital intelligence capture for visitor behavior analytics (Hosted Tag Version 1.5.2) | All pages |
| 7 | **Video Marketing Platform (NNI Video)** | Embed/Video | Medium | `nni-video.videomarketingplatform.co` — Novo Nordisk's video platform with GTM integration via glueframe and datalayer scripts | Pages with video content |
| 8 | **CryptoJS** | Library/Security | Low | `cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/crypto-js.min.js` — Client-side cryptography library, likely for form encryption or token generation | Forms/eligibility pages |
| 9 | **iAssist (Enrollment Platform)** | API/External | Very High | `novocare.iassist.com` — External enrollment and consent platform for patient program enrollment (MASH consent form, patient authorization) | https://www.novocare.com/mash/home.html |
| 10 | **Novo Nordisk Prescribing Information** | External Links | Low | `novo-pi.com` — Links to prescribing information PDFs and medication guides for all products | All product pages (ISI panels) |
| 11 | **FDA MedWatch** | External Links | Low | `fda.gov/medwatch` — FDA adverse event reporting links in ISI panels | All product pages |
| 12 | **OneTrust Privacy Portal** | External/API | Low | `privacyportal.onetrust.com` — Privacy rights request webform | Footer on all pages |
| 13 | **Diabetes Education Subdomain** | External Subdomain | High | `diabeteseducation.novocare.com` — Separate site with different template, nav structure, content hub with article cards, topic filters, diabetes type selector, and Spanish language support | https://www.novocare.com/diabetes/diabetes-education.html (redirects) |
| 14 | **jQuery** | Library | Low | jQuery loaded via AEM granite client libraries — used for DOM manipulation across components | All pages |

### AEM Infrastructure Details

| Component | Details |
|-----------|---------|
| **AEM Version** | AEM as a Cloud Service |
| **Template** | `brandbase-novocare-page-template` (from meta tag) |
| **Client Libraries** | `brandbase/common/clientlibs`, `brandbase/novocare/clientlibs`, `nnicloud-patient/components`, `novo-core-framework/site/components` |
| **jQuery** | Loaded via `clientlibs/granite/jquery` |
| **Component Framework** | Custom Novo Nordisk "brandbase" framework with "novo-core-framework" and "nnicloud-patient" overlays |

---

## 5. Complex Use Cases & Observations

### 5.1 Important Safety Information (ISI) System

- **Instances:** Every product-related page (~150+ pages)
- **Where:** All therapeutic area pages, product pages, check coverage pages
- **Why it's complex:** ISI panels are extensive (thousands of words per product), must be legally accurate, support expand/collapse behavior, include scroll FAB navigation, and multiple ISI panels can stack on a single page (e.g., Wegovy + Saxenda on obesity page, 6 products on bleeding disorders page). Content includes structured headings, bold warnings, bulleted side effects, PI/Medication Guide PDF links, and FDA reporting links. ISI content is FDA-regulated and must be pixel-perfect.

### 5.2 Multi-Therapeutic-Area Architecture with Audience Segmentation

- **Instances:** 7 therapeutic areas x 2 audiences (patient + HCP) = 14 experience paths
- **Where:** Entire site structure
- **Why it's complex:** Each therapeutic area has its own navigation, content hierarchy, product set, and ISI requirements. Patient and HCP experiences run in parallel with different content emphasis. The obesity/weight loss section uses a completely different template and navigation pattern (hamburger menu vs tab nav) from all other therapeutic areas. URL redirect patterns vary (most areas redirect `/{area}.html` to `/{area}/home.html`, but obesity redirects to `/patient/home.html`).

### 5.3 Insurance Information Content Replication

- **Instances:** ~50 pages across 5 therapeutic areas
- **Where:** `/diabetes/insurance-information/`, `/obesity/insurance-information/`, `/growth-related-disorders/insurance-information/`, `/bleeding-disorders/insurance-information/`, `/ph1/insurance-information/`
- **Why it's complex:** Six "Exploring Insurance" sub-pages and four "Insurance Types" sub-pages are structurally identical across 5 therapeutic areas but may have area-specific content nuances. This creates a content management challenge — updates need to propagate across all instances. Ideal candidate for shared content fragments or experience fragments in migration.

### 5.4 Eligibility Forms and External Enrollment System

- **Instances:** 16+ eligibility form pages
- **Where:** `/eligibility/` path (myinsulinrx, savings cards, PAP, pharmacy enrollment, etc.)
- **Why it's complex:** Forms integrate with `novocare.iassist.com` external enrollment platform. Multi-step form flows with eligibility validation logic, insurance status branching, terms acceptance, and CryptoJS encryption. Each therapeutic area has distinct eligibility criteria and form fields. SMS terms pages suggest text message enrollment flows.

### 5.5 Diabetes Education Subdomain

- **Instances:** 20+ pages on separate subdomain
- **Where:** `diabeteseducation.novocare.com`
- **Why it's complex:** Entirely separate site with different template system, navigation structure, content hub layout with article cards, topic filter icons, diabetes type selector (Type 1/Type 2/Not sure), and Spanish language support via `espanol.cornerstones4care.com`. This is effectively a second site that would need its own migration plan.

### 5.6 Product-Specific Warning Labels and Categorization

- **Instances:** All product-related pages
- **Where:** Health warning banners, ISI panels, sub-navigation
- **Why it's complex:** Different products require different warning categories, ISI content, and PI links. The site dynamically shows/hides ISI panels based on the product context. Some pages show ISI for multiple products simultaneously (bleeding disorders: 6 ISI panels). Warning content is legally mandated and varies by indication.

### 5.7 Spanish Language Content

- **Instances:** 7 pages (bleeding disorders only)
- **Where:** `/content/novocare/es/bleeding-disorders/`
- **Why it's complex:** Only one therapeutic area has Spanish translations, using AEM's `/content/novocare/es/` language copy path. Inconsistent multilingual support creates questions about future language expansion requirements during migration.

### 5.8 Hidden Sections / Conditional Content

- **Instances:** Multiple homepage-level pages
- **Where:** Homepage, disease-area landing pages
- **Why it's complex:** Console logs reveal `Showing hidden sections [next, obesity-inactive]` and `Decoding hidden section` messages, indicating client-side conditional content display logic. Sections may be shown/hidden based on user state, A/B testing, or feature flags.

---

## 6. Migration Estimates

### Complexity Assessment

| Factor | Rating | Justification |
|--------|--------|---------------|
| Template Count | Medium-High | 10 templates, but 3-4 variants of therapeutic area home |
| Component Count | Medium | 28 components, most are content-focused (cards, text, ISI) |
| Page Volume | High | 214 pages, but ~50 are templated insurance info (automatable) |
| Interactive Features | Medium | Condition selector, medicine selector, tab interfaces, accordions |
| Third-Party Integrations | High | 12+ integrations including dual analytics (Adobe + Google), enrollment platform, video platform |
| Content Complexity | Very High | FDA-regulated ISI content, multi-product safety info, legal compliance |
| Forms/Enrollment | Very High | 16+ eligibility forms with external iAssist integration |
| Multilingual | Low | Only 7 Spanish pages (bleeding disorders) |
| Subdomain | High | Separate diabeteseducation.novocare.com site |

### Effort Breakdown

| Phase | Estimated Days | Details |
|-------|---------------|---------|
| **Discovery & Planning** | 8–10 | Template analysis, ISI content audit, form workflow mapping, integration documentation, subdomain scoping |
| **Design System Migration** | 6–8 | Novo Nordisk brand system, NovoCare color palette, typography, responsive patterns, therapeutic area color coding |
| **Global Components** | 8–12 | Header variants (patient/HCP), footer, sub-navigation tabs, cookie consent, ISI panel system with expand/collapse and FAB |
| **Homepage & Hub Pages** | 4–6 | Global homepage with condition selector, HCP hub with card grid, Contact Us |
| **Therapeutic Area Homes** | 10–14 | 6 therapeutic area home pages with varied layouts (multi-product, single-product, obesity variant), step-by-step walkthrough, tabbed insurance process |
| **Content Sub-Pages** | 8–12 | Help with costs, savings offers, product pages, check coverage — card-based layouts with ISI |
| **Insurance Information** | 4–6 | ~50 templated pages — high automation potential with shared content fragments |
| **Eligibility Forms** | 12–16 | 16+ form pages with iAssist integration, validation logic, multi-step flows, encryption |
| **Pharmacy Section** | 5–7 | Pharmacy landing, product-specific pharmacy pages, pricing table, FAQ accordion |
| **HCP Section** | 6–8 | 25 HCP pages mirroring patient structure with different content emphasis |
| **ISI Content Migration** | 6–8 | 20+ unique ISI content sets with legally mandated accuracy requirements, expand/collapse behavior |
| **Integration Migration** | 6–8 | Adobe Launch, GTM, GA4, Bing Ads, OneTrust, NNI Video, iAssist enrollment, CryptoJS |
| **Spanish Content** | 2–3 | 7 pages, bleeding disorders only |
| **QA & Testing** | 8–10 | Cross-browser, accessibility, ISI content accuracy verification, form testing, analytics validation |
| **TOTAL** | **85–130** | **person-days** |

### Risk Factors

1. **ISI Legal Compliance:** ISI content is FDA-regulated. Any migration must preserve exact wording, formatting, and link accuracy. Legal review is required for every migrated page with ISI content.
2. **iAssist Integration Complexity:** The external enrollment platform integration requires API documentation and may involve authentication, session management, and encrypted data transfer.
3. **Diabetes Education Subdomain:** The `diabeteseducation.novocare.com` site is effectively a separate migration project with its own template system, content hub, and Spanish language support.
4. **Hidden Section Logic:** Client-side conditional content display may be tied to A/B testing, personalization, or feature flags that need to be replicated or replaced.
5. **Dual Analytics Stack:** Running both Adobe Launch and Google Tag Manager adds complexity to analytics migration — need to determine if both are required in the target architecture.
6. **Form Encryption:** CryptoJS usage in forms suggests client-side encryption that needs careful handling during migration.

### Migration Recommendation

**Phase 1 (Quick Wins — Weeks 1-4):**
- Migrate ~50 insurance information pages (highly templated, automatable)
- Migrate Contact Us and simple content pages (~15 pages)
- Set up global components (header, footer, ISI system)

**Phase 2 (Core Pages — Weeks 5-10):**
- Migrate therapeutic area home pages (6 pages)
- Migrate product sub-pages and check coverage pages (~30 pages)
- Migrate HCP section (25 pages)

**Phase 3 (Complex Features — Weeks 11-16):**
- Migrate eligibility forms with iAssist integration (16+ pages)
- Migrate pharmacy section (6 pages)
- Migrate weight loss/obesity section (unique template)

**Phase 4 (Subdomain & Polish — Weeks 17-20):**
- Assess diabeteseducation.novocare.com migration (separate project)
- Spanish content migration
- Final QA, analytics validation, and ISI legal review

---

*Report generated by Adobe Professional Services — April 2, 2026*
