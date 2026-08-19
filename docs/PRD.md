# Product Requirements Document

## TravelApp 

---

# 1. Executive Summary

A comprehensive trip workspace and intelligent travel companion covering the entire trip lifecycle. It seamlessly connects geography (space) and timeline (time)—empowering travelers to intuitively explore and build itineraries before the trip, navigate and execute on the road as an active guide, collaborate effortlessly with co-travelers, and dynamically adapt to real-time changes or intelligent suggestions on the fly.

---

# 2. Problem Statement

Planning and executing a trip is an exercise in tool fragmentation, cognitive overload, and rigid static plans. Travelers lack a unified platform that acts as a single source of truth across the full trip lifecycle—from pre-trip discovery and collaborative itinerary design to in-trip execution, dynamic adaptation, and post-trip reflection. This fragmentation creates hurdles throughout every stage of the journey:

1. **Tool Fragmentation & Context Switching** — Travelers cobble together disparate tools across different phases—maps for geography, sheets for itineraries, messaging apps for collaboration, other apps for weather and safety alerts. This forces manual, redundant effort and makes it hard to keep one cohesive, up-to-date plan accessible at a glance.

2. **The Core Planning Problem: Spatial + Temporal Disconnect** — What travelers actually do today during trip planning is fundamentally a process of **Spatial + Temporal Planning**. They are constantly attempting to solve a multi-dimensional puzzle simultaneously:
   - **Spatial awareness (Where things are):** Understanding the geographic layout of attractions, dining, viewpoints, and transit points.
   - **Temporal constraints (How long they take):** Accounting for visit durations, opening/operating hours, and realistic travel times between stops.
   - **Clustering & Flow (What can be grouped together):** Identifying which POIs logically belong on the same day to minimize transit overhead.
   - **Lodging Anchors (Where to stay):** Deciding where it makes strategic sense to sleep based on the evolving itinerary, rather than picking hotels in a vacuum.
   - **Ripple Effects (What happens when something moves):** Understanding the cascading consequences on travel time, day feasibility, and lodging when any single item is added, moved, or rescheduled.

   Today, these two dimensions live in separate, disconnected tools:
   - **The geographic dimension** lives in navigation/map apps (e.g., Google Maps), which are great for point lookups and navigation but weak for early, flexible, pre-itinerary planning.
   - **The temporal dimension** lives in spreadsheets, calendar apps, or text notes, which track days and times but lack spatial awareness and automatic routing feedback.

   Because neither tool bridges space and time, the traveler's brain is forced to act as the manual calculation engine—juggling tabs, estimating drive times, recalculating day loads, and rebuilding itineraries from scratch whenever a plan changes.

3. **Collaborative & Social Friction** — Sharing trip plans stays disjointed, buried in long messaging threads or static emails. Collecting traveler feedback and suggestions during the planning phase is messy. Coordinating changes during the trip, tracking shared expenses (and pay-back calculations), and managing real-time location sharing during the trip creates logistical friction and social tension.

4. **The "Planning vs. Execution" Usability Gap** — Planning often happens on desktop; execution happens on mobile, often with limited connectivity. Current tools offer weak offline support, leaving travelers stranded without itinerary or navigation details. Desktop-first planning documents also don't translate well to actionable mobile companions on the move.

5. **Lack of In-Trip Dynamic Adaptation & Real-Time Intelligence** — Once on the road, travelers operate with static plans that cannot adapt to real-world disruptions (delays, fatigue, weather shifts, traffic, attraction closures, or spontaneous discoveries). Missing: an active companion that can serve as a live guide for the planned route while also offering **fluid real-time adjustment**—calculating the cascading ripple effects of in-trip deviations, and proactively generating contextual recommendations and alternative options without requiring the traveler to manually rebuild their schedule.

---

# 3. Target Platforms

Three primary platforms, for a seamless experience across devices:

1. **Web App** — a robust interface for deep planning, trip configuration, and data management.
2. **Android App** — a mobile-first companion for execution, real-time navigation, and on-the-go updates.
3. **iPhone App** — a mobile-first companion for execution, real-time navigation, and on-the-go updates.

---

# 4. Product Vision & Principles

## 4.1 Product Vision: Full Lifecycle Travel Platform

A unified visual workspace and intelligent companion built on **Spatial + Temporal Continuity** across the entire trip lifecycle. The product bridges geography (space) and timeline (time)—taking travelers seamlessly from initial inspiration to on-the-road execution and beyond. It directly addresses the problems identified in §2 across all core lifecycle stages:

### 1. Stage 1: Pre-Trip Planning (Spatial + Temporal Canvas)
An intuitive, interactive planning board where travelers explore places of interest, visualize them on a map, cluster them into logical days, and dynamically experiment with routes. The system continuously resolves the core planning puzzle:
- **Spatial Awareness:** Understanding what is near what across destinations.
- **Clustering & Flow:** Grouping places logically into daily schedules to minimize transit waste.
- **Lodging Anchors:** Strategically placing accommodations based on the route rather than booking in isolation.
- **Temporal Feasibility:** Calculating transit times, activity durations, and free time to instantly surface whether a day is balanced or overloaded.
- **Ripple Effects:** Visualizing cascading impacts across the itinerary whenever an attraction or stay is moved, added, or deleted.

### 2. Stage 2: Sharing & Collaborative Co-Creation (Social Synchronization)
A single source of truth that eliminates disjointed chat threads, scattered links, and messy spreadsheets:
- **Pre-Trip Collaboration:** Co-creating itineraries with co-travelers, allowing group members to propose places, vote on activities, and view changes in real time.
- **Shared Budget & Expense Tracking:** Built-in tracking for group expenses, split costs, and automated pay-back calculations.
- **In-Trip Social Coordination:** Seamless sharing of live locations, itineraries, and meeting points among travel companions to remove logistical friction on the road.

### 3. Stage 3: Actual Trip & Live Execution (In-Pocket Mobile & Offline Guide)
Bridging the desktop-to-mobile usability gap with a high-utility, mobile-first travel companion:
- **Robust Offline Resilience:** Full access to maps, schedules, notes, and bookings in areas with limited or no cellular connectivity.
- **Active Itinerary Execution:** Guiding travelers smoothly from activity to transit to lodging with turn-by-turn routing, timing context, and daily progress tracking.
- **Contextual Access:** Storing all confirmation details, tickets, and location-specific notes directly where and when they are needed.

### 4. Stage 4: Run-Time Adjustments & Dynamic Adaptation (Adaptive In-Trip Co-Pilot)
Empowering travelers when reality inevitably diverges from the plan (weather shifts, unexpected closures, delays, traffic, fatigue, or spontaneous opportunities):
- **Fluid On-The-Fly Editing:** Allowing travelers to easily swap, postpone, or drop activities with instant recalculation of ripple effects across the rest of the day and trip.
- **Contextual Real-Time Intelligence:** Proactively suggesting smart alternatives (e.g., indoor activities during sudden rain, nearby dining recommendations, detour adjustments for road closures) without forcing travelers to manually rebuild their plans.

### 5. Stage 5: Post-Trip Reflection & Archiving (Resolution & Memory Canvas)
A clean closure experience to wrap up the journey:
- **Actuals vs. Plan:** Preserving the recorded route, actual timeline, and visited places for memories or future reference.
- **Financial Settlement:** Finalizing shared expense balances and exportable summaries.
- **Reusability:** Transforming past trips into reusable templates or shareable recommendations for friends and the community.

---

## 4.2 Key Product Principles

1. **"Every change is visible in both space and time."**
   Whether dragging an attraction to a new day during desktop planning or shifting an afternoon stop on mobile while stuck in traffic, all changes immediately update across both the map and timeline with fresh travel times, day loads, and feasibility indicators.

2. **"Optimize and augment the user's thinking, not replace it."**
   The product gives travelers clarity, empowerment, and control. Rather than an opaque "black box" that dictates rigid schedules, the system provides transparent calculations, consequences, and proactive suggestions so *the user* remains the ultimate decision-maker (e.g., *"If you spend 1 more hour here, you'll reach stop #4 after closing—here are 2 alternate options nearby"*).

3. **"Frictionless Collaboration & Single Source of Truth."**
   The entire travel group operates from one unified, dynamic workspace—combining planning, sharing, expense splitting, and live status in one place instead of scattered across multiple siloed apps.

4. **"Seamless Desktop Planning to Resilient In-Pocket Execution."**
   A unified data model ensures that the rich, expressive canvas crafted on the web translates into a dependable, offline-ready mobile guide that executes and dynamically adapts on the go.

---

# 5. Target Audience & User Personas

| Persona | Description | Key Needs | Pain Points |
| :--- | :--- | :--- | :--- |
| **Solo backpacker / independent multi-day traveler** | Plans trips of several days or more — road trips, multi-city/region trips, trips with many attractions, trips where geography matters a lot to the plan. Wants control over the plan, not the system building the trip for them. | Understand the geographic structure of a trip quickly; understand daily load quickly; compare alternatives; change the route without redoing manual work; reliable guide on the road | Juggling maps, spreadsheets, and notes; hard to tell what's realistic to fit in a day; losing track of travel-time cost between stops; difficulty adapting when plans change on-trip |
| **Group travelers** | [ ]  | [ ] | [ ] |

---

# 6. Goals & Objectives

## 6.1 Business Goals
- [ ]

## 6.2 User Goals
- **Pre-Trip:** Quickly understand the geographic structure of a trip and evaluate if days are realistic or overloaded.
- **Pre-Trip:** Experiment with routes, cluster activities, align lodging, and see ripple effects instantly without manual rework.
- **Pre-Trip:** Compare multiple route/day alternatives before committing.
- **In-Trip:** Rely on a clear, offline-ready mobile guide for navigation, timing, and daily schedule execution.
- **In-Trip:** Adapt effortlessly to real-time changes (delays, weather, closures) with instant schedule recalculation and intelligent alternative suggestions.
- **Post-Trip:** Review trip actuals and resolve shared expenses without friction.

## 6.3 Non-Goals
The MVP is explicitly *not* an "AI Travel Planner" — it should not fully auto-generate an itinerary or make decisions for the user without their control.

---

# 7. Success Metrics / KPIs

- How easily a user goes from "I have 30 places I'm interested in" to "I understand what this trip could look like"
- Fast understanding of the trip's geographic structure
- Fast understanding of each day's load
- Changing the route without manual rework
- Early detection of problems in the route
- Ability to compare multiple alternatives
- A feeling of control, not a feeling of a "black box"

---

# 8. Scope

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
| FR-13 | Dynamic route planning factoring in drive times, daily limits, and lodging needs | [ ] | [ ] | Idan — problem statement §2(5). Overlaps with Asaf's "Future Direction" list — likely the same feature described from two angles. |
| FR-14 | Proactive recommendations based on preferences, weather, and local events | [ ] | [ ] | Idan — problem statement §2(5). Same overlap as above. |
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

Two connected spaces —
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

---

# 18. Assumptions & Constraints

## Assumptions
- Users don't necessarily want the system to fully build the trip for them — they want control over planning, with the system providing information, calculations, and consequences.

## Constraints
- [ ]

---

# 19. Risks & Mitigations

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
