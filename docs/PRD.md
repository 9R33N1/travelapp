# Product Requirements Document

## TravelApp *(temporary name)*

> ### ⚠️ Read this first — the core scope question
> Asaf's doc describes a tightly scoped **map + timeline planning canvas**, with an MVP that explicitly avoids AI/automation and doesn't mention collaboration, booking, expenses, or real-time location.
> Idan's PRD problem statement describes a much bigger **all-in-one trip platform** — covering collaboration, shared expenses, real-time location sharing, offline execution mode, weather, and post-trip archiving, in addition to planning. It's also already scoped against real competitors (Wanderlog, TripIt) that operate at that broader scale.
> Both are valid products, but they're different bets on what to build first — and notably, Idan's own competitive analysis (§8.3) shows Wanderlog already does something close to Asaf's MVP *and* the collaboration layer. Worth discussing directly. Called out again in §21.

---

# 1. Executive Summary

**Asaf:** "A visual trip-planning workspace for Spatial + Temporal Planning that seamlessly connects geography and time—allowing travelers to explore places, group them into days, experiment with routes, and instantly understand the ripple effects of every planning decision."

---

# 2. Problem Statement

## 2.1 Shared framing (Idan)

Planning a trip is an exercise in app juggling: research lives in chats, itineraries in spreadsheets, and navigation in map apps. Travelers lack a unified platform that acts as a single source of truth for all trip-related data — including flights, accommodations, transportation, weather forecasts, maps, dining, and activity recommendations. This fragmentation creates hurdles throughout the trip lifecycle:

1. **Tool Fragmentation & Context Switching** — Travelers cobble together disparate tools to organize a trip — maps for geography, sheets for itineraries, messaging apps for collaboration, other apps for weather and safety alerts. This forces manual, redundant effort and makes it hard to keep one cohesive plan accessible at a glance.

2. **The "Planning vs. Execution" Usability Gap** — Planning often happens on desktop; execution happens on mobile, often with limited connectivity. Current tools offer weak offline support, leaving travelers stranded without itinerary or navigation details. Desktop-first planning documents also don't translate well to mobile screens on the move.

3. **Collaborative & Social Friction** — Sharing trip plans stays disjointed, buried in long messaging threads or static emails. Coordinating changes, tracking shared expenses (and pay-back calculations), and managing real-time location sharing during the trip creates logistical friction and social tension.

4. **Lack of Dynamic & Contextual Intelligence** — Travelers operate with static plans that can't adapt to the real world. Missing: **dynamic route planning** that factors in drive times, daily limits, and accommodation needs; **real-time intelligence** — proactive, AI-generated recommendations based on preferences, current weather, and local events (road closures, wildfires, accidents); **fluid adjustment** — the ability to adjust routes/plans on the fly without manually reconstructing the itinerary.

## 2.2 Core Planning Dynamics: Spatial + Temporal Planning (Asaf)

What travelers actually do today during trip planning is fundamentally a process of **Spatial + Temporal Planning**. They are constantly attempting to solve a multi-dimensional puzzle simultaneously:
- **Spatial awareness (Where things are):** Understanding the geographic layout of attractions, dining, viewpoints, and transit points.
- **Temporal constraints (How long they take):** Accounting for visit durations, opening/operating hours, and realistic travel times between stops.
- **Clustering & Flow (What can be grouped together):** Identifying which POIs logically belong on the same day to minimize transit overhead.
- **Lodging Anchors (Where to stay):** Deciding where it makes strategic sense to sleep based on the evolving itinerary, rather than picking hotels in a vacuum.
- **Ripple Effects (What happens when something moves):** Understanding the cascading consequences on travel time, day feasibility, and lodging when any single item is added, moved, or rescheduled.

Today, these two dimensions live in separate, disconnected tools:
- **The geographic dimension** lives in navigation/map apps (e.g., Google Maps), which are great for point lookups and navigation but weak for early, flexible, pre-itinerary planning.
- **The temporal dimension** lives in spreadsheets, calendar apps, or text notes, which track days and times but lack spatial awareness and automatic routing feedback.

Because neither tool bridges space and time, the traveler's brain is forced to act as the manual calculation engine—juggling tabs, estimating drive times, recalculating day loads, and rebuilding itineraries from scratch whenever a plan changes.

---

# 3. Target Platforms

Three primary platforms, for a seamless experience across devices:

1. **Web App** — a robust interface for deep planning, trip configuration, and data management.
2. **Android App** — a mobile-first companion for execution, real-time navigation, and on-the-go updates.
3. **iPhone App** — a mobile-first companion for execution, real-time navigation, and on-the-go updates.

---

# 4. Product Vision & Principles

**Asaf — Vision:** A visual tool designed specifically for **Spatial + Temporal Planning**—letting a traveler build a trip as an interactive planning board that seamlessly connects geography (space) and timeline (time). Users add places of interest, visualize them on the map, cluster them into days, and dynamically "play" with their schedule. The product answers the five core spatial-temporal questions simultaneously:
- **Spatial awareness:** What's near what?
- **Clustering:** Which places make sense to do on the same day?
- **Lodging anchors:** Where should I stay based on the route?
- **Temporal budget:** How long will each day take, how much time is lost to transit, and is the day overloaded?
- **Ripple effects:** What happens across the whole route if I move an attraction or change where I sleep?

**Asaf — Key principle:** *"The product should optimize the user's thinking, not replace it."* Instead of saying "here's your optimal trip," the product should say something like: "If you do these things today, it'll take 8h20m, of which 2h10m is travel, leaving you 1 free hour." The system isn't meant to decide the trip for the user — it's meant to give them information, calculations, and consequences so *they* can decide.

> Note: this principle sits in some tension with Idan's problem-statement point on "proactive, AI-generated recommendations" (§2.1, point 4). Not a hard contradiction — Asaf frames intelligence/automation as a later layer on top of a user-controlled core, not a core MVP feature. Worth aligning on explicitly — see §21.

---

# 5. Target Audience & User Personas

| Persona | Description | Key Needs | Pain Points |
| :--- | :--- | :--- | :--- |
| **Solo backpacker / independent multi-day traveler** *(Idan's persona, filled in with Asaf's description)* | Plans trips of several days or more — road trips, multi-city/region trips, trips with many attractions, trips where geography matters a lot to the plan. Wants control over the plan, not the system building the trip for them. | Understand the geographic structure of a trip quickly; understand daily load quickly; compare alternatives; change the route without redoing manual work | Juggling maps, spreadsheets, and notes; hard to tell what's realistic to fit in a day; losing track of travel-time cost between stops |
| **Group travelers** *(Idan)* | [ ] *(Idan's persona — description not yet written; likely tied to the collaboration/expense-splitting features in §2.1(3), which are outside Asaf's MVP — see §8)* | [ ] | [ ] |

---

# 6. Goals & Objectives

## 6.1 Business Goals
- [ ]

## 6.2 User Goals
- Quickly understand the geographic structure of a trip (what's near what)
- Quickly understand whether a given day is realistic or overloaded
- Be able to change the plan (move something to another day) and immediately see the impact, without manually redoing the route
- Compare multiple route/day alternatives before committing
- Decide where to stay based on the plan, not the other way around

## 6.3 Non-Goals
**Asaf:** The MVP is explicitly *not* an "AI Travel Planner" — it should not fully auto-generate an itinerary or make decisions for the user without their control.

---

# 7. Success Metrics / KPIs

| Goal | Metric / KPI | Target | Measurement Source |
| :--- | :--- | :--- | :--- |
| [ ] | [ ] | [ ] | [ ] |

**Asaf — qualitative success criteria** *(not yet expressed as measurable KPIs — worth converting into the table above once you agree on targets):*
- How easily a user goes from "I have 30 places I'm interested in" to "I understand what this trip could look like"
- Fast understanding of the trip's geographic structure
- Fast understanding of each day's load
- Changing the route without manual rework
- Early detection of problems in the route
- Ability to compare multiple alternatives
- A feeling of control, not a feeling of a "black box"

---

# 8. Scope

## ⚠️ Key scope question (see callout at top of doc)
Before filling this in for real: decide whether v1 is Asaf's focused planning-canvas MVP, with Idan's broader platform features as later phases — or whether you're building toward the full platform (and competing head-on with Wanderlog — see §8.3) from day one. The lists below are drafted assuming the *phased* approach (Asaf's MVP = in scope now, Idan's broader items = later), but that's an assumption, not a decision.

## 8.1 In Scope (draft — Asaf's MVP)
| In Scope |
| :--- |
| Create a Trip |
| Add Places |
| Show Places on a map |
| Create Days |
| Drag & drop Places between days |
| Timeline view per day |
| Automatic travel-time calculation |
| Automatic duration / free-time calculation |
| Add Hotels |
| Two-way sync between Map and Timeline |
| Day load / feasibility indicator |
| Instantly see the impact of changing the route |

## 8.2 Out of Scope / Later Phases (draft)
| Out of Scope (for now) | Source |
| :--- | :--- |
| AI-generated itinerary / full automation of trip building | Asaf (explicit non-goal) |
| Suggested attraction clusters, suggested lodging, optimal-order suggestions, "gap" detection, restaurant suggestions near current location, opening-hours & weather awareness, multiple auto-generated alternatives | Asaf ("Future Direction" — intended as an intelligence layer on top of the core, not the product itself) |
| Multi-user collaboration / shared trip editing | Idan (problem statement, not in Asaf's MVP) |
| Shared expense tracking & pay-back calculations | Idan |
| Real-time location sharing during the trip | Idan |
| Offline mode for execution phase | Idan |
| Live booking / reservations for flights & hotels; email-parsed itinerary import (à la TripIt) | Idan |
| Weather & local-event awareness (closures, wildfires, accidents) | Idan |
| Post-trip archiving / actuals-vs-plan | Idan |

## 8.3 Competitive context
Worth reading alongside the scope question above: **Wanderlog** already does a version of both the map+timeline canvas (Asaf's MVP) *and* the collaboration/route-optimization layer (Idan's broader scope), free, across Web/iOS/Android. **TripIt** competes on a different axis — automated itinerary building from forwarded confirmation emails, aimed at frequent/business travelers, monetizing via real-time flight alerts. Neither doc currently states a differentiated wedge against Wanderlog specifically — that's worth a direct answer before locking scope. Full detail in §22.2.

---

# 9. Core Objects / Data Model (conceptual)

*Unique contribution from Asaf's doc — Idan's PRD doesn't yet define a data model. Worth reviewing together, especially if broader-platform items (bookings, expenses, collaboration) end up in scope, since those will need their own entities.*

- **Place** — anything the user is interested in (Attraction, Restaurant, Hotel, City, Hike, etc.)
- **Activity** — a planned visit to a Place. Includes duration, preferred time, opening hours/constraints, priority, notes.
- **Travel Segment** — the transition between two activities. Includes distance, travel time, transportation mode.
- **Day** — the core planning unit. Includes date, start/end, activities, travel, hotel, free time.
- **Stay** — a lodging location, connected to one or more days.

---

# 10. User Journeys

1. **Planning & Preparation** — initial discovery and (if in scope) collaborative phase where users research destinations, build the itinerary, and manage bookings.

   1. **Explore** — user adds/collects places of interest
   2. **Map** — all places appear on the map to reveal the geographic structure
   3. **Cluster** — user identifies or creates geographic groupings (D1, D2, D3, ...)
   4. **Assign** — places get assigned to specific days
   5. **Optimize** — the system calculates travel times, durations, and load, and lets the user play with the order
   6. **Commit** — once the route stabilizes, it becomes a final itinerary

   The experience should be gradual and should not require a complete itinerary up front.

2. **In-Transit / Execution** — active travel phase relying on real-time navigation, live updates, and offline access to execute the plan. *(Depends on the scope decision in §8 — offline support is not part of Asaf's MVP list.)*

3. **On-Trip Management** — daily experience during the trip: collaborative updates, expense tracking, real-time social/location sharing. *(Depends on the scope decision in §8 — not part of Asaf's MVP list.)*

4. **Post-Trip Reflection & Archiving** — capturing actuals vs. plan, finalizing expense splits, storing trip memories/data for future reference. *(Depends on the scope decision in §8.)*

---

# 11. Key Interaction Principle

**"Every change should be visible in both space and time."**

Because trip planning is an ongoing **Spatial + Temporal Planning** process, any action taken on the canvas must immediately reflect across both dimensions.

Example: the user drags an attraction from Day 3 to Day 4. The system immediately recalculates and visually updates:
- its geographic position and sequence on the Day 4 map route
- the chronological order of activities on the Day 4 timeline
- point-to-point travel times and transit legs
- activity start/end times
- remaining free time and overall day load / feasibility indicator
- lodging proximity and whether the chosen hotel/stay still makes sense

This lets the user run effortless "what if we did this tomorrow instead?" experiments without having to manually recalculate drive times or rebuild the entire route.

---

# 12. User Stories / Use Cases

| ID | As a... | I want to... | So that... | Priority |
| :--- | :--- | :--- | :--- | :--- |
| US-01 | independent traveler | see all my saved places on a map | I understand the geographic structure of my trip | [Must / Should / Could] |
| US-02 | independent traveler | drag a place from one day to another | I can instantly see how it affects travel time and day load | [Must / Should / Could] |
| US-03 | [ ] | [ ] | [ ] | [ ] |

---

# 13. Functional Requirements

| ID | Requirement | Platform | Priority | Source / Notes |
| :--- | :--- | :--- | :--- | :--- |
| FR-01 | Create a trip | [ ] | [ ] | Asaf — MVP |
| FR-02 | Add places to a trip | [ ] | [ ] | Asaf — MVP |
| FR-03 | Display places on an interactive map | [ ] | [ ] | Asaf — MVP |
| FR-04 | Create/manage days within a trip | [ ] | [ ] | Asaf — MVP |
| FR-05 | Drag & drop places between days | [ ] | [ ] | Asaf — MVP |
| FR-06 | Per-day timeline view (Travel → Activity → Travel → Activity → Hotel) | [ ] | [ ] | Asaf — MVP |
| FR-07 | Automatic travel-time calculation between activities | [ ] | [ ] | Asaf — MVP |
| FR-08 | Automatic duration & free-time calculation per day | [ ] | [ ] | Asaf — MVP |
| FR-09 | Add hotels/stays, linked to one or more days | [ ] | [ ] | Asaf — MVP |
| FR-10 | Two-way sync: changes on the map reflect on the timeline and vice versa | [ ] | [ ] | Asaf — MVP |
| FR-11 | Day load / feasibility indicator | [ ] | [ ] | Asaf — MVP |
| FR-12 | Instant recalculation of route/time impact when the plan changes | [ ] | [ ] | Asaf — MVP |
| FR-13 | Dynamic route planning factoring in drive times, daily limits, and lodging needs | [ ] | [ ] | Idan — problem statement §2.1(4). Overlaps with Asaf's "Future Direction" list — likely the same feature described from two angles. |
| FR-14 | Proactive recommendations based on preferences, weather, and local events | [ ] | [ ] | Idan — problem statement §2.1(4). Same overlap as above. |
| FR-15 | [ ] | [ ] | [ ] | [ ] |

---

# 14. Non-Functional Requirements

| Category | Requirement |
| :--- | :--- |
| Performance | [ ] |
| Scalability | [ ] |
| Security & Privacy | [ ] *(note: real-time location sharing, if in scope, has real privacy implications worth scoping carefully — see §21)* |
| Accessibility | [ ] |
| Localization / i18n | [ ] *(note: source material for this project is bilingual — Hebrew/English — worth deciding target market language(s) explicitly)* |
| Offline Support | Idan's problem statement flags this as a key gap in existing tools during the execution phase — not yet defined as a requirement; depends on scope decision in §8. |
| Compatibility (browsers, OS versions, devices) | [ ] |
| Reliability / Availability | [ ] |

---

# 15. User Experience & Design

**Asaf's core screen concept:** two connected spaces —
- **Map** — interactive map showing all relevant places (Attractions, Restaurants, Hotels, Cities, Hikes, Viewpoints, other POIs), which can be color/style-coded by type, day, status, or area.
- **Timeline / Trip Board** — a timeline divided by day, visually showing Travel → Activity → Travel → Activity → Hotel, with start time, duration, location, travel time, notes, and time constraints per activity.

## User Flows
[Link to flow diagrams]

## Wireframes / Mockups
[Link to Figma / design file]

## Design Guidelines
[Link to design system / brand guidelines]

---

# 16. Technical Considerations

## Architecture Overview
[High-level architecture, link to technical design doc]

## APIs & Integrations
List third-party services this app will depend on (e.g., maps, geolocation, travel-time calculation, weather, push notifications, analytics, and — if in scope — booking/inventory providers, email parsing, and payment processing for expense splitting).
- [ ]

## Data & Privacy
[Data collected, storage, retention, compliance considerations (e.g., GDPR, CCPA). If real-time location sharing (Idan) ends up in scope, this needs explicit treatment — location data is sensitive.]

---

# 17. Dependencies

| Dependency | Type (Internal / External / Third-Party API) | Owner | Status |
| :--- | :--- | :--- | :--- |
| [ ] | [ ] | [ ] | [ ] |

---

# 18. Assumptions & Constraints

## Assumptions
- Users don't necessarily want the system to fully build the trip for them — they want control over planning, with the system providing information, calculations, and consequences.

## Constraints
- [ ]

---

# 19. Risks & Mitigations

| Risk | Likelihood | Impact | Mitigation |
| :--- | :--- | :--- | :--- |
| [ ] | [Low/Med/High] | [Low/Med/High] | [ ] |

---

# 20. Launch Plan

## Rollout Strategy
[Phased rollout, beta, feature flags, regional launch, etc.]

## Go-to-Market
[Marketing, App Store / Play Store listing, PR, support readiness]

---

# 21. Open Questions

| # | Question | Owner | Status |
| :--- | :--- | :--- | :--- |
| 1 | Do we build Asaf's focused planning-canvas MVP first, with Idan's broader platform (collaboration, expenses, booking, real-time location, offline mode) as later phases — or design for the full platform from the start? | Idan & Asaf | Open |
| 2 | Given Wanderlog already covers both the canvas *and* the collaboration layer for free — what's our differentiated wedge? | Idan & Asaf | Open |
| 3 | Is any form of AI/automated recommendation part of the MVP, or strictly a post-MVP layer? | Idan & Asaf | Open |
| 4 | Is multi-user collaboration (shared trip editing) in scope for v1? | Idan & Asaf | Open |
| 5 | Is live booking / email-parsed itinerary import (flights/hotels) in scope, or is the app planning-only? | Idan & Asaf | Open |
| 6 | Is offline support required for launch, or can it come later? | Idan & Asaf | Open |
| 7 | Platform sequencing — build web first and add mobile after, or launch on all three together? | Idan & Asaf | Open |
| 8 | What's the monetization / business model? (Both Wanderlog and TripIt use freemium — worth deciding early whether we follow that model.) | [ ] | Open |
| 9 | [ ] | [ ] | Open |

---

# 22. Appendix

## 22.1 Current Tools & Solutions Ecosystem 
- **Navigation & Mapping** (e.g., Google Maps) — route optimization, discovery and recommendations (lodging, points of interest, dining), real-time location sharing, turn-by-turn navigation. Strong for navigation and point lookups; weaker for early-stage, pre-itinerary planning. *(Idan + Asaf)*
- **Email clients** (e.g., Gmail) — central repository for travel confirmation details: flights, hotel reservations, rental cars *(Idan)*
- **Note-taking apps** (e.g., Google Keep) — quick notes, lists, informal recommendations
- **Documents & spreadsheets** (e.g., Google Docs, Google Sheets) — custom itinerary creation, budget management, structured trip tracking
- **Social platforms** (Facebook, Instagram) — crowdsourced recommendations and inspiration for attractions, dining, accommodations
- **Messaging & communication** (WhatsApp, iMessage) — direct communication, group coordination, ad-hoc sharing of locations/itineraries/ideas
- **Weather services** — monitoring destination forecasts and conditions
- **Rideshare services** — local transportation and point-to-point transit booking
- **Printed maps** — still used in practice for early-stage planning *(Asaf)*

## 22.2 Market Landscape & Core Competitors

**1. Wanderlog**
- Core value: closest thing to "Google Docs for travel" — combines chronological day-by-day itineraries with a live interactive map.
- Functionality: drop places of interest onto a map, optimize routes, collaborate live with friends, manage travel budgets.
- Platform: full data sync across Web, iOS, Android.
- Pricing: freemium — core itinerary mapping/editing/collaboration is free; Pro unlocks offline access, email auto-forwarding, and direct export to Google Maps.
- *Relevant to §21, Q2 — this is the closest existing product to both Asaf's canvas MVP and Idan's collaboration layer, and it's free.*

**2. TripIt**
- Core value: master itinerary automation for frequent/business travelers.
- Functionality: scans a linked inbox or forwarded confirmation emails (flights, hotels, rental cars) to auto-compile a chronological trip.
- Platform: Web dashboard, iOS, Android.
- Pricing: freemium — automated email parsing and basic timelines are free; TripIt Pro adds real-time flight delay alerts, gate changes, alternate flight finder.

## 22.3 Future Direction — post-MVP intelligence layer
- Suggested groupings of attractions
- Suggested lodging locations
- Detection of overloaded days
- Suggested optimal ordering
- Detection of "gaps" in the route
- Restaurant suggestions near the user's current area
- Awareness of opening hours
- Weather awareness
- User preference awareness
- Generating multiple route alternatives
