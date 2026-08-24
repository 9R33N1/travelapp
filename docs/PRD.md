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

# 3. Product Vision & Principles

## 3.1 Product Vision: Full Lifecycle Travel Platform

TravelApp is a single workspace that keeps a trip's geography and timeline in sync — from the first place a traveler saves, through planning with co-travelers, through execution on the road, to looking back afterward. Instead of a plan going stale the moment it's written, the product treats it as something living: every edit, whether made on a desktop map weeks before departure or on a phone mid-trip, updates the same underlying model and is immediately reflected everywhere.

Four ideas anchor that:

- **Space and time are one model, not two.** Where things are and how long they take are calculated together, always — never a map view and a schedule view that can drift out of sync.
- **Planning and execution are the same product, not a handoff.** The itinerary a traveler builds on the web is the same one that guides them on mobile, offline if needed — no export, no rebuild.
- **Collaboration is built in, not bolted on.** A trip has one shared source of truth co-travelers plan, coordinate, and split costs against, rather than reconstructing the plan across chats and spreadsheets.
- **The system informs; the traveler decides.** It surfaces consequences and alternatives — never silently auto-generates or overrides the plan.

---

## 3.2 Key Product Principles

1. **"Every change is visible in both space and time."**
   Whether dragging an attraction to a new day during desktop planning or shifting an afternoon stop on mobile while stuck in traffic, all changes immediately update across both the map and timeline with fresh travel times, day loads, and feasibility indicators.

2. **"Optimize and augment the user's thinking, not replace it."**
   The product gives travelers clarity, empowerment, and control. Rather than an opaque "black box" that dictates rigid schedules, the system provides transparent calculations, consequences, and proactive suggestions so *the user* remains the ultimate decision-maker (e.g., *"If you spend 1 more hour here, you'll reach stop #4 after closing—here are 2 alternate options nearby"*).

3. **"Frictionless Collaboration & Single Source of Truth."**
   The entire travel group operates from one unified, dynamic workspace—combining planning, sharing, expense splitting, and live status in one place instead of scattered across multiple siloed apps.

4. **"Seamless Desktop Planning to Resilient In-Pocket Execution."**
   A unified data model ensures that the rich, expressive canvas crafted on the web translates into a dependable, offline-ready mobile guide that executes and dynamically adapts on the go.

---

# 4. Target Audience & User Personas

### 4.1 Solo Backpacker / Independent Multi-Day Traveler
- **Description:** Plans trips of several days or more (road trips, multi-city/region trips, trips with many attractions where geography matters a lot to the plan). Wants control over the plan, not the system building the trip for them.
- **Key Needs:** Understand the geographic structure of a trip quickly; understand daily load quickly; compare alternatives; change the route without redoing manual work; reliable guide on the road.
- **Pain Points:** Juggling maps, spreadsheets, and notes; hard to tell what's realistic to fit in a day; losing track of travel-time cost between stops; difficulty adapting when plans change on-trip.

### 4.2 Group Travelers (2 or More Co-Travelers)
- **Description:** Two or more people traveling together (friends, couples, families) who need to coordinate planning, align during the trip, and manage logistics together.
- **Key Needs:**
  - **Shared Planning Process:** A collaborative workspace to propose places, vote/align on activities, and build a unified itinerary without chaotic message threads.
  - **Real-Time Information Sharing:** Instant sync of schedule changes on the road, access to shared logistics (stays, bookings, meeting points), and live coordination/status during the trip.
  - **Shared Expense Management:** Transparent logging of group expenses (fuel, lodging, food, activities) and automated calculation of splits and settlements (who owes whom).
  - **Single Source of Truth:** One shared home for the trip instead of scattering information across WhatsApp, spreadsheets, and Splitwise.
- **Pain Points:** Scattered communication and lost recommendations in chat apps; burden falling on a single organizer; confusion when plans change mid-trip; awkwardness and manual math around splitting costs.

---

# 5. Goals & Objectives

## 5.1 Business Goals
- [ ]

## 5.2 User Goals
- **Pre-Trip:** Quickly understand the geographic structure of a trip and evaluate if days are realistic or overloaded.
- **Pre-Trip:** Experiment with routes, cluster activities, align lodging, and see ripple effects instantly without manual rework.
- **Pre-Trip:** Compare multiple route/day alternatives before committing.
- **Pre-Trip (Group):** Seamlessly co-create itineraries with co-travelers without conflicting edits or fragmented communication.
- **In-Trip:** Rely on a clear, offline-ready mobile guide for navigation, timing, and daily schedule execution.
- **In-Trip:** Adapt effortlessly to real-time changes (delays, weather, closures) with instant schedule recalculation and intelligent alternative suggestions.
- **Post-Trip:** Review trip actuals and resolve shared expenses without friction.

---

# 6. Target Platforms

Three primary platforms, for a seamless experience across devices:

- **Web App** — a robust interface for deep planning, trip configuration, and data management.
- **Android App** — a mobile-first companion for execution, real-time navigation, and on-the-go updates.
- **iPhone App** — a mobile-first companion for execution, real-time navigation, and on-the-go updates.

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

# 8. Scope & MVP Definition

## 8.1 In Scope (MVP: Core Spatial + Temporal Planning Canvas)
- **Create a Trip:** Create and manage trips with destinations and date ranges.
- **Add Places:** Add and manage places/POIs with duration estimates and notes.
- **Interactive Map:** Display all saved places with visual indicators for assigned days and categories.
- **Timeline View:** Per-day timeline showing sequence: `Start/Lodging -> Travel -> Activity -> Travel -> Activity -> End/Lodging`.
- **Drag & Drop:** Reorder places within a day or move places between days.
- **Automatic Calculations:** Automatic calculation of point-to-point travel times, activity durations, and free time.
- **Lodging Anchors:** Add hotels/stays linked to one or more days, with automatic route transit calculation.
- **Two-Way Sync:** Bidirectional synchronization between Map and Timeline.
- **Day Load Indicator:** Visual feedback on day feasibility (balanced vs. overloaded).
- **Ripple Effect Updates:** Instant recalculation of downstream impact when any part of the route changes.

## 8.2 Out of Scope / Later Phases
- **AI Itinerary Generation:** Full automated generation of trip plans (explicit non-goal).
- **Post-MVP Intelligence Layer:** Proactive POI clustering, lodging suggestions, TSP route optimization, route gap detection, nearby dining recommendations, opening-hours & weather awareness.
- **Group Collaboration:** Multi-user live co-editing, voting, and role permissions.
- **Shared Expenses:** In-app expense logging and debt settlement calculation.
- **Real-Time Location Sharing:** Live location tracking and rendezvous coordination during the trip.
- **Offline Mode:** Full offline sync and execution.
- **Bookings & Email Parsing:** Direct flight/hotel booking integration or email reservation import (TripIt style).
- **Post-Trip Archiving:** Actuals vs. plan comparison and trip memory export.

---

# 9. Core Objects / Data Model (conceptual)

- **Place** — anything the user is interested in (Attraction, Restaurant, Hotel, City, Hike, etc.)
- **Activity** — a planned visit to a Place. Includes duration, preferred time, opening hours/constraints, priority, notes.
- **Travel Segment** — the transition between two activities. Includes distance, travel time, transportation mode.
- **Day** — the core planning unit. Includes date, start/end, activities, travel, hotel, free time.
- **Stay** — a lodging location, connected to one or more days.

---

# 10. User Journeys

1. **Planning & Preparation** — initial discovery and itinerary building:
   - **Explore:** User adds/collects places of interest.
   - **Map:** All places appear on the map to reveal geographic structure.
   - **Cluster:** User identifies geographic groupings across days.
   - **Assign:** Places are assigned to specific days.
   - **Optimize:** The system calculates travel times, durations, and load; user refines the sequence.
   - **Commit:** The route stabilizes into a working itinerary.
   *(The experience is gradual and does not require a complete itinerary up front.)*

2. **In-Transit / Execution** — active travel phase relying on navigation and schedule execution.

3. **On-Trip Management** — daily experience during the trip: collaborative updates, expense tracking, real-time coordination.

4. **Post-Trip Reflection & Archiving** — capturing actuals vs. plan, finalizing expenses, saving memories.

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

# 12. Functional Requirements *(MVP)*

- **FR-01:** Create a trip 
- **FR-02:** Add places to a trip 
- **FR-03:** Display places on an interactive map 
- **FR-04:** Create/manage days within a trip 
- **FR-05:** Drag & drop places between days 
- **FR-06:** Per-day timeline view (Travel → Activity → Travel → Activity → Hotel) 
- **FR-07:** Automatic travel-time calculation between activities 
- **FR-08:** Automatic duration & free-time calculation per day 
- **FR-09:** Add hotels/stays, linked to one or more days 
- **FR-10:** Two-way sync: changes on the map reflect on the timeline and vice versa 
- **FR-11:** Day load / feasibility indicator 
- **FR-12:** Instant recalculation of route/time impact when the plan changes 

---

# 13. Non-Functional Requirements

- **Performance:** [ ]
- **Scalability:** [ ]
- **Security & Privacy:** [ ] *(Note: real-time location sharing, if in scope, has real privacy implications worth scoping carefully)*
- **Accessibility:** [ ]
- **Localization / i18n:** [ ] *(Note: source material is bilingual Hebrew/English)*
- **Offline Support:** Identified as a key gap in existing execution tools; to be phased into mobile execution.
- **Compatibility:** [ ] (Browsers, OS versions, devices)
- **Reliability / Availability:** [ ]

---

# 14. User Experience & Design

Two connected spaces:
- **Map** — interactive map showing all relevant places (Attractions, Restaurants, Hotels, Cities, Hikes, Viewpoints, other POIs), color/style-coded by type, day, status, or area.
- **Timeline / Trip Board** — a timeline divided by day, visually showing Travel → Activity → Travel → Activity → Hotel, with start time, duration, location, travel time, notes, and time constraints per activity.

## User Flows
[Link to flow diagrams]

## Wireframes / Mockups
[Figma Design File](https://www.figma.com/design/wG3BGW8S89Ot1oh4EpgKIj/Untitled?node-id=0-1&t=KRFWxFkSCgVVT095-1)

## Design Guidelines
[Link to design system / brand guidelines]

---

# 15. Technical Considerations

## Architecture Overview
[High-level architecture, link to technical design doc]

## APIs & Integrations
List third-party services this app will depend on (e.g., maps, geolocation, travel-time calculation, weather, push notifications, analytics, booking/inventory providers, email parsing, payment processing for expense splitting):
- [ ]

## Data & Privacy
[Data collected, storage, retention, compliance considerations (e.g., GDPR, CCPA). Location data requires explicit privacy treatment.]

---

# 16. Dependencies & Assumptions

## 16.1 Dependencies
- Third-party mapping, routing, and geolocation services (e.g., Mapbox, Google Maps API).

## 16.2 Assumptions
- Users want control over planning, with the system providing information, calculations, and consequences rather than an automated black box that decides for them.

---

# 17. Risks & Mitigations

- **Risk:** [ ] *(Likelihood: [Low/Med/High], Impact: [Low/Med/High], Mitigation: [ ])*

---

# 18. Launch Plan

## Rollout Strategy
[Phased rollout, beta, feature flags, regional launch, etc.]

## Go-to-Market
[Marketing, App Store / Play Store listing, PR, support readiness]

---

# 19. Open Questions

1. **Scope priority:** Do we build the focused planning-canvas MVP first, with broader platform features (collaboration, expenses, booking, real-time location, offline mode) as later phases — or design for the full platform from the start?
2. **Competitive wedge:** Given Wanderlog already covers both the canvas and the collaboration layer for free — what is our differentiated wedge? 
3. **AI role:** Is any form of AI/automated recommendation part of the MVP, or strictly a post-MVP layer?
4. **Collaboration:** Is multi-user collaboration (shared trip editing) in scope for v1?
5. **Bookings:** Is live booking / email-parsed itinerary import (flights/hotels) in scope, or is the app planning-only?
6. **Offline:** Is offline support required for launch, or can it come later?
7. **Platforms:** Platform sequencing — build web first and add mobile after, or launch on all three together?
8. **Monetization:** What is the monetization / business model?

---

# 20. Appendix

## 20.1 Current Tools & Solutions Ecosystem
- **Navigation & Mapping** (e.g., Google Maps) — route optimization, discovery and recommendations (lodging, POIs, dining), real-time location sharing, turn-by-turn navigation. Strong for navigation and point lookups; weaker for early-stage, pre-itinerary planning.
- **Email Clients** (e.g., Gmail) — central repository for travel confirmation details (flights, hotel reservations, rental cars).
- **Note-Taking Apps** (e.g., Google Keep, Apple Notes) — quick notes, lists, informal recommendations.
- **Documents & Spreadsheets** (e.g., Google Docs, Google Sheets) — custom itinerary creation, budget management, structured trip tracking.
- **Social Platforms** (Facebook, Instagram, TikTok) — crowdsourced recommendations and inspiration for attractions, dining, accommodations.
- **Messaging & Communication** (WhatsApp, iMessage) — direct communication, group coordination, ad-hoc sharing of locations/itineraries/ideas.
- **Expense Splitting Apps** (e.g., Splitwise) — group expense tracking and bill splitting.
- **Weather Services** — monitoring destination forecasts and conditions.
- **Rideshare Services** — local transportation and point-to-point transit booking.
- **Printed Maps** — still used in practice for early-stage geographic planning.

## 20.2 Market Landscape & Competitive Context

### 1. Wanderlog
- **Core Value:** Closest thing to "Google Docs for travel" — combines chronological day-by-day itineraries with a live interactive map.
- **Functionality:** Pin places of interest on a map, optimize routes, collaborate live with friends, manage travel budgets.
- **Platform:** Full data sync across Web, iOS, Android.
- **Pricing:** Freemium — core itinerary mapping/editing/collaboration is free; Pro unlocks offline access, email auto-forwarding, and direct export to Google Maps.
- **Competitive Context & Opportunity:** Wanderlog is the closest existing product to both our canvas and collaboration layer. Our differentiator focuses on superior spatial-temporal fluidity, deterministic ripple-effect modeling, and staying an empowering planning canvas rather than a document-heavy text layout.

### 2. TripIt
- **Core Value:** Master itinerary automation for frequent/business travelers.
- **Functionality:** Scans a linked inbox or forwarded confirmation emails (flights, hotels, rental cars) to auto-compile a chronological trip.
- **Platform:** Web dashboard, iOS, Android.
- **Pricing:** Freemium — automated email parsing and basic timelines are free; TripIt Pro adds real-time flight delay alerts, gate changes, alternate flight finder.
- **Competitive Context & Opportunity:** TripIt is reactive to already-booked reservations; it does not solve early-stage spatial exploration, manual route design, or leisure day planning.

### 3. Rhyme (formerly Roamy) — [rhyme.travel](https://www.rhyme.travel/)
- **Core Value:** Turns social-media inspiration into a finished trip. Positioned as "you save the spots, we'll handle the rest" — the opposite end of the automation spectrum from our "optimize the user's thinking, not replace it" principle (§3.2).
- **Functionality:** Imports saved spots from Instagram, TikTok, Google Maps links, and screenshots and auto-detects the location; organizes them into shareable lists by city/vibe/trip; shows everything on a live map; then an AI itinerary builder generates a full day-by-day route from selected lists, dates, and destination. Supports inviting friends to a shared trip so co-travelers can each add their must-see spots before the AI builds the plan.
- **Platform:** iOS live now; Android listed as "pre-order" (not yet launched).
- **Pricing:** Free to download and save spots; Pro subscription (monthly/annual) required for unlimited AI itinerary generation. App Store and Play Store reviews raise recurring complaints about surprise annual charges after the free trial and generic/repetitive AI itinerary suggestions (e.g., over-clustering one activity type) — worth noting as a trust/pricing-transparency pitfall to avoid, not just a feature gap to close.
- **Competitive Context & Strategic Relevance:** Rhyme is the sharpest existing example of the "system decides" end of the spectrum that our Non-Goals (§5.3) explicitly reject. This makes it a useful reference point when writing and refining intelligence and recommendation requirements (FR-13/FR-14 in §12, and §19 Open Questions) so we remain deliberate about how much automation we actually want, and where.

## 20.3 Future Direction — Post-MVP Intelligence Layer
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
