# RTT Landing Page — Initial Design & Layout Directions
**STAR Health | Byte Development**
**Prepared by:** Samuel Moloney
**Date:** February 2026
**Status:** Draft for Client Review

---

## Design Philosophy

The RTT page must project **authority without aggression**. The target audience (law enforcement, protective services, emergency responders) instinctively trust clean, structured, precise communication — not sensationalism. The aesthetic should feel closer to a high-end tactical medical brand than a military surplus site.

**Three words to guide every decision:** Credible. Controlled. Capable.

---

## Colour Palette

| Role | Colour | Hex | Usage |
|---|---|---|---|
| Primary Dark | Charcoal | `#1C1C1E` | Backgrounds, headers, dominant text |
| Primary Mid | Steel Blue | `#2C4A6E` | Section backgrounds, anchor colour |
| Accent | Amber Gold | `#C8882A` | CTAs, highlights, key stats |
| Neutral Light | Off-White | `#F5F4F0` | Page background, card backgrounds |
| Text | Dark Slate | `#2D2D2D` | Body copy |
| Subtle | Mid Grey | `#8A8A8A` | Secondary text, captions |

**Rationale:** The charcoal/steel blue pairing reads as serious and institutional (consistent with emergency services). Amber gold adds warmth and urgency to CTAs without resorting to red (which skews military/danger). Off-white keeps it breathable and far from gore aesthetics.

---

## Typography

| Element | Font | Weight | Notes |
|---|---|---|---|
| Page Title / Hero H1 | Barlow Condensed | 700 (Bold) | All caps, wide tracking |
| Section Headings H2 | Barlow Condensed | 600 (SemiBold) | Mixed case |
| Sub-headings H3 | Inter | 600 (SemiBold) | Standard case |
| Body Copy | Inter | 400 (Regular) | 16–18px, generous line-height |
| Labels / Tags | Inter | 500 (Medium) | Small caps, letter-spaced |
| CTAs | Inter | 700 (Bold) | Uppercase |

**Rationale:** Barlow Condensed carries weight and authority in headings without feeling decorative. Inter is the gold standard for clean, readable body text across screen sizes.

---

## Page Layout — Section by Section

### 1. Hero Section

```
┌─────────────────────────────────────────────────────────────┐
│                    [FULL-WIDTH DARK OVERLAY]                 │
│           Background: Training photo (team-based,            │
│                   controlled environment)                    │
│                                                              │
│   REALITY TRAUMA TRAINING                                    │
│   ─────────────────────────────────────                     │
│   Specialised trauma response training for those             │
│   who operate where standard first aid ends.                 │
│                                                              │
│   [ ENQUIRE ABOUT RTT TRAINING ]   [ ↓ Learn More ]         │
│                                                              │
│   ● Nationally Accredited  ● Scenario-Based  ● Closed-Group  │
└─────────────────────────────────────────────────────────────┘
```

**Specs:**
- Full viewport height (100vh)
- Background: Full-bleed training photo with a charcoal overlay at ~60% opacity
- H1: Large Barlow Condensed, white, all caps
- Subheadline: Inter Regular, off-white, ~20px
- Primary CTA: Amber gold button, dark text — "ENQUIRE ABOUT RTT TRAINING"
- Secondary CTA: Ghost/outline button — "Learn More" with scroll arrow
- Trust signals: Three short credential/feature pills along the bottom of the hero
- **Photo Direction:** Team of 2–3 participants in a controlled training scenario. No visible weapons or blood. Strong lighting. Neutral/industrial background.

---

### 2. "What Is RTT?" — Intro Strip

```
┌─────────────────────────────────────────────────────────────┐
│  [STEEL BLUE BACKGROUND]                                     │
│                                                              │
│  WHAT IS REALITY TRAUMA TRAINING?                            │
│                                                              │
│  RTT is a closed-group, scenario-driven program designed     │
│  for professionals who may encounter traumatic injury        │
│  in high-stakes operational environments. Built around       │
│  real-world scenarios — including edged weapon and           │
│  ballistic trauma — this training goes beyond standard       │
│  first aid to build genuine response capability under        │
│  pressure.                                                   │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

**Specs:**
- Steel blue background, white text
- Single column, centred, max-width 780px
- Short, punchy — 3–4 sentences max
- No imagery needed here; text carries the section

---

### 3. Key Differentiators / UVP Block

```
┌─────────────────────────────────────────────────────────────┐
│  [OFF-WHITE BACKGROUND]                                      │
│                                                              │
│        WHY STAR HEALTH RTT?                                  │
│                                                              │
│  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐      │
│  │  [Icon]       │ │  [Icon]       │ │  [Icon]       │      │
│  │               │ │               │ │               │      │
│  │ Scenario-     │ │ Specialist    │ │ Nationally    │      │
│  │ Based         │ │ Instructors   │ │ Accredited    │      │
│  │               │ │               │ │               │      │
│  │ Real-world    │ │ Led by        │ │ Meets         │      │
│  │ trauma        │ │ experienced   │ │ compliance    │      │
│  │ scenarios     │ │ practitioners │ │ requirements  │      │
│  └───────────────┘ └───────────────┘ └───────────────┘      │
│                                                              │
│  ┌───────────────┐ ┌───────────────┐                        │
│  │  [Icon]       │ │  [Icon]       │                        │
│  │               │ │               │                        │
│  │ Closed-Group  │ │ Adaptive      │                        │
│  │ Delivery      │ │ Curriculum    │                        │
│  │               │ │               │                        │
│  │ Private &     │ │ Tailored to   │                        │
│  │ confidential  │ │ your role &   │                        │
│  │ cohorts       │ │ environment   │                        │
│  └───────────────┘ └───────────────┘                        │
└─────────────────────────────────────────────────────────────┘
```

**Specs:**
- Off-white background
- 3-column grid (wraps to 1-column on mobile)
- Each card: minimal icon (line art), bold heading, 1–2 sentence description
- No borders — use generous whitespace to separate cards
- Icons: Clean, professional line-art style (not playful or cartoon)

---

### 4. Who This Is For — Audience Block

```
┌─────────────────────────────────────────────────────────────┐
│  [CHARCOAL BACKGROUND]                                       │
│                                                              │
│      BUILT FOR THOSE WHO OPERATE IN HIGH-RISK               │
│      ENVIRONMENTS                                            │
│                                                              │
│   ● Law Enforcement & Police Services                        │
│   ● Protective & Close Protection Services                   │
│   ● Military & Defence Personnel                             │
│   ● Emergency Medical Services                               │
│   ● Fire & Rescue Services                                   │
│   ● Critical Infrastructure Security Teams                   │
│                                                              │
│                                                              │
│   [Photo: Instructor demonstrating to a small group]         │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

**Specs:**
- Charcoal background with white text
- Two-column layout: copy/list on left, training photo on right
- Use a simple checkmark or dash list (no bullet emojis)
- Photo: Instructor in a hands-on demonstration scenario. Clean environment, professional attire.
- Flip column order on mobile (photo on top)

---

### 5. Training Overview / What's Covered

```
┌─────────────────────────────────────────────────────────────┐
│  [OFF-WHITE BACKGROUND]                                      │
│                                                              │
│      WHAT THE TRAINING COVERS                                │
│                                                              │
│  ┌──────────────────────────────┐                           │
│  │  Haemorrhage Control         │  [Expand +]               │
│  └──────────────────────────────┘                           │
│  ┌──────────────────────────────┐                           │
│  │  Penetrating Trauma Response │  [Expand +]               │
│  └──────────────────────────────┘                           │
│  ┌──────────────────────────────┐                           │
│  │  Airway Management           │  [Expand +]               │
│  └──────────────────────────────┘                           │
│  ┌──────────────────────────────┐                           │
│  │  Scenario-Based Simulations  │  [Expand +]               │
│  └──────────────────────────────┘                           │
│  ┌──────────────────────────────┐                           │
│  │  Team-Based Response Drills  │  [Expand +]               │
│  └──────────────────────────────┘                           │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

**Specs:**
- Accordion-style expandable list
- Off-white background
- Each row: module name + expand icon
- Expanded state: 2–3 sentence description of module content
- Keep it clean — no imagery needed here
- **Note:** Exact module list to be confirmed with Thomas

---

### 6. Enquiry / CTA Section

```
┌─────────────────────────────────────────────────────────────┐
│  [STEEL BLUE BACKGROUND]                                     │
│                                                              │
│      ENQUIRE ABOUT RTT TRAINING                              │
│                                                              │
│   RTT courses are delivered to closed groups only.           │
│   To discuss training for your team or organisation,         │
│   submit an enquiry below.                                   │
│                                                              │
│   ┌──────────────────┐  ┌──────────────────┐               │
│   │  Name            │  │  Organisation    │               │
│   └──────────────────┘  └──────────────────┘               │
│   ┌──────────────────┐  ┌──────────────────┐               │
│   │  Email           │  │  Phone           │               │
│   └──────────────────┘  └──────────────────┘               │
│   ┌───────────────────────────────────────────┐             │
│   │  Role / Team Size / Training Requirements  │             │
│   │                                           │             │
│   └───────────────────────────────────────────┘             │
│                                                              │
│            [ SUBMIT ENQUIRY ]                                │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

**Specs:**
- Steel blue background, white text
- Clean, minimal form — 5 fields max
- CTA button: Amber gold, dark text, full-width on mobile
- Micro-copy beneath button: "All enquiries are handled confidentially."
- Form submission: Connects to Thomas's email / CRM (to be confirmed)

---

### 7. Footer (Shared with Main Site)

- STAR Health logo
- Navigation links
- Contact info
- Accreditation logos
- Copyright

---

## Imagery Direction Summary

Since Thomas is still sourcing photography, the following shot list should guide that process:

| Shot | Description | Do | Don't |
|---|---|---|---|
| Hero | Team in training scenario | 2–3 people, clinical environment, neutral background | Visible weapons, excessive blood, military gear |
| Instructor | Hands-on teaching moment | Close-up of hands demonstrating technique | Posed/stiff poses |
| Group | Small cohort listening to briefing | Engaged participants, professional attire | Large crowds, casual clothing |
| Detail | Medical equipment/kit | Tourniquet, gauze, gloves on a surface | Graphic wound imagery |

**Lighting:** Natural or soft studio lighting. Avoid harsh flash or high-contrast "action cam" look.

---

## Mobile Considerations

- All multi-column layouts collapse to single column
- Hero text scale reduces to remain readable without overflow
- CTA button becomes full-width
- Accordion module list is ideal for mobile (avoids long scroll walls)
- Navigation: Hamburger menu (shared with main site)

---

## Next Steps

1. **Thomas:** Confirm RTT module list for Section 5 (Training Overview)
2. **Thomas:** Provide first batch of training photography
3. **Samuel:** Confirm website platform with Dom before proceeding to high-fidelity mockup
4. **Samuel:** Produce Figma wireframes once platform is confirmed
5. **All:** Review and sign off on this direction before design execution begins

---

*This document represents initial layout and design directions only. Final designs are subject to client feedback, platform constraints, and asset availability.*
