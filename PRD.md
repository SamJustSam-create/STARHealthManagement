# Product Requirements Document (PRD)

## Project Name: STAR Health Website Update & E-Commerce Integration
**Client:** STAR Health (Thomas)
**Developer/Agency:** Byte Development (Samuel Moloney)
**Original Date:** February 2026
**Last Updated:** May 2026

### Revision History
| Date | Revision |
|---|---|
| February 2026 | Initial PRD authored. |
| May 2026 | Reconciled with project status as of 2026-05-12: added Homepage (§4.3) and Fire Safety Training Page (§4.4) deliverables. Action items (§6) refreshed against actual project state including delivered wireframes, image batch one, and current outstanding items. WhatsApp confirmed as primary client channel (email to Dom was non-functional). |

## 1. Project Overview
The objective of this project is to update the STAR Health website to prominently feature their specialized Reality Trauma Training (RTT) for emergency responders, while maintaining a professional and accessible tone for their general first aid and fire safety courses. Additionally, an e-commerce shop will be integrated natively into the website, ensuring users remain on the same domain during their shopping experience.

## 2. Target Audience
* **Primary (RTT Courses):** Emergency services, law enforcement, protective services, and other specialized first responder roles.
* **Secondary (General Courses):** The general public and corporate clients seeking nationally accredited first aid and fire safety training. *(Note: Publicly available RTT courses are not planned for 2026).*

## 3. Brand & Tone Guidelines
The brand must walk a fine line between showcasing realistic trauma training and remaining approachable to the general public.
* **Vibe:** Professional, credible, controlled, and clean. 
* **Visuals:** Scenario-based training imagery, hands-on trauma care, team-based training shots, utilizing strong lighting and neutral grading.
* **What to Emphasize:** The Unique Value Proposition (UVP) — delivering excellent, "reality-based training scenarios" for trauma-related injuries (e.g., edged weapons, ballistic/gunshot wounds).
* **What to Avoid:** Overly military aesthetics, excessive gore, or "over-the-top" violence (guns/blood) that could turn away the general public.
* **General Landing Page:** Must utilize a "softer" approach to welcome everyday users seeking standard nationally accredited courses.

## 4. Key Features & Deliverables

### 4.1. RTT (Reality Trauma Training) Landing Page
* **Purpose:** A dedicated, specialized page to market closed-source courses to law enforcement and first responders.
* **Content Strategy:** Clearly articulate the UVP (reality-based training) without alienating the broader state/country audience.
* **Media Integration:** Integration of specific, well-lit, professional training photos (either staged locally or licensed stock imagery). The client is currently organizing these assets.

### 4.2. Native E-Commerce Shop
* **Purpose:** A dedicated shop page built with the focus and conversion strategy of a landing page.
* **Requirement:** The e-commerce experience must be kept entirely on the same website, preventing users from being navigated to a separate site/domain.
* **Coordination:** Development and structure to be collaborated on with team member "Dom".

### 4.3. Homepage
* **Purpose:** The primary public-facing entry point for the site, balancing the credibility of RTT with approachability for the general public seeking standard first aid and fire safety training.
* **Added:** Scope expanded post-PRD on Thomas's request (2026-03-19) to include the homepage and a clearer route to courses offered / upcoming courses.
* **Status:** Initial wireframe delivered 2026-03-31 (`wireframes/homepage-wireframe.html`). Client feedback received; awaiting incorporation of imagery and minor nav fixes.
* **Open question:** "About SHM" / "Learn More About Us" buttons currently link to each other — pending Thomas's decision on whether to build a dedicated About page or strip the buttons.

### 4.4. Fire Safety Training Page
* **Purpose:** A dedicated page championing the fire safety training offering, mirroring the structural depth of the RTT page but with a softer, public-facing tone suitable for corporate and general audiences.
* **Added:** Scope expanded post-PRD on Thomas's request (2026-05-08).
* **Unique Value Proposition:** SHM's ability to deliver training on-site at the client's premises (mobile delivery). This is to be the page's headline hook.
* **Positioning:** To sit alongside RTT in the primary navigation as a co-equal pillar, rather than nested under the general nationally-accredited courses.
* **Coordination:** Course specifics (modules, durations, accreditation, pricing) to be provided by Dom. Photography direction (on-site / mobile delivery imagery) to be provided by Enrique once course scope is confirmed.
* **Status:** Proposal acknowledged with client (2026-05-12); awaiting course information from Dom before wireframing.

## 5. Technical Requirements
* **Platform Integration:** The shop must be natively integrated into the current site architecture. Given the existing Shopify store (`https://30263c-69.myshopify.com/`), this will likely be achieved via a Shopify Headless integration (e.g., Shopify Storefront API) to keep users on the same domain.
* **Media Assets:** Imagery must be high-resolution. Staged smartphone photography is acceptable provided it has excellent lighting, resolution, and framing.

## 6. Action Items

### Outstanding
* **Thomas (STAR Health):** Confirm page positioning for the new Fire Safety Training Page (co-equal with RTT in nav) and whether it should have a dedicated enquiry form or feed into the general contact form.
* **Thomas (STAR Health):** Clarify the amendments and additions to the "Why STAR Health RTT?" UVP boxes (feedback raised 2026-03-31; not yet actioned pending the confirmed list).
* **Thomas (STAR Health):** Decide whether to build a dedicated About page or strip the "About SHM" / "Learn More About Us" buttons from the homepage nav.
* **Thomas / Enrique (STAR Health):** Deliver the second batch of higher-quality course photography (anticipated post-2026-05-04 course; not yet received as of last sit-rep).
* **Dom (STAR Health):** Provide Shopify Storefront API tokens to enable the headless shop integration (originally requested 2026-03-11).
* **Dom (STAR Health):** Provide fire safety course specifics — modules, durations, accreditation, pricing — to enable wireframing of the Fire Safety Training Page.
* **Enrique (STAR Health):** Once fire safety course scope is confirmed by Dom, provide on-site / mobile delivery photography aligned with the "we come to you" USP.
* **Samuel (Byte Dev):** Once Dom delivers course information, produce the Fire Safety Training Page wireframe (~1 week turnaround committed in 2026-05-12 sit-rep).

### Completed
* **Samuel (Byte Dev):** Initiate contact with Dom for e-commerce shop planning. *(Note: Email channel to Dom was non-functional; the SHM social media WhatsApp group was created on 2026-03-02 as the primary working channel and remains so.)*
* **Dom (STAR Health):** Confirmed the existing platform (Shopify — `https://30263c-69.myshopify.com/`) and shared the full product catalogue for review.
* **Samuel (Byte Dev):** Presented initial design and layout directions for the RTT page incorporating the "clean and professional" aesthetic constraints.
* **Samuel (Byte Dev):** Delivered three site wireframes — Homepage, RTT page, and Shop page — hosted via GitHub Pages and reviewed with the client.
* **Samuel (Byte Dev):** Provided specific image dimension requirements to Enrique for all hero, product, and content imagery (2026-03-31). See `Image-Assets-Spec.md`.
* **Enrique (STAR Health):** Delivered first batch of four Canva-approved images for use on the site (2026-05-07).
* **Samuel (Byte Dev):** Issued project sit-rep and Fire Safety Training Page proposal to client (2026-05-12).
