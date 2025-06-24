# 🚧 ExploreSF Backlog

This backlog is structured for use with Windsurf and includes Epics, User Stories, and Implementation Milestones.

---

## 🧭 EPIC 1: User Onboarding & Profile Management

**Goal:** Enable users to register, set preferences, and personalize their experience.

### User Stories:
- **US-1.1**: As a user, I want to sign up using email or social login so I can access the app securely.
- **US-1.2**: As a user, I want to set my age, location, and mood so the app can tailor recommendations.
- **US-1.3**: As a user, I want to select interests and preferred categories during onboarding.
- **US-1.4**: As a user, I want to update my preferences anytime from the settings panel.
- **US-1.5**: As a user, I want my location to be detected automatically to show nearby events.

---

## 🔎 EPIC 2: Event Discovery & Search

**Goal:** Allow users to explore, filter, and search events.

### User Stories:
- **US-2.1**: As a user, I want to search for events using a freeform text bar.
- **US-2.2**: As a user, I want to filter events by category, vibe, cost, time, and distance.
- **US-2.3**: As a user, I want to see a list and map view of nearby events.
- **US-2.4**: As a user, I want to see tags (e.g., "Black-owned", "Rooftop") to explore niche interests.
- **US-2.5**: As a user, I want to view event details including venue, time, price, and RSVP options.

---

## 🧠 EPIC 3: Personalized Recommendations

**Goal:** Generate AI-based recommendations based on context and preferences.

### User Stories:
- **US-3.1**: As a user, I want to get personalized recommendations based on my interests and past behavior.
- **US-3.2**: As a user, I want to set my mood (e.g., chill, adventurous) and get suggestions accordingly.
- **US-3.3**: As a user, I want a "Surprise Me" button that curates an unexpected but relevant itinerary.
- **US-3.4**: As a user, I want recommendations that adjust to the time of day and weather.

---

## 🌐 EPIC 4: External Data Integrations

**Goal:** Integrate and ingest external data from third-party sources.

### User Stories:
- **US-4.1**: As a developer, I want to pull event data from the Eventbrite API.
- **US-4.2**: As a developer, I want to sync business and venue data from Yelp Fusion.
- **US-4.3**: As a developer, I want to pull free event feeds from SF Funcheap RSS.
- **US-4.4**: As a developer, I want to enrich events with weather data via OpenWeatherMap.
- **US-4.5**: As a content manager, I want to manually submit or approve community-submitted events.

---

## ❤️ EPIC 5: User Interactions

**Goal:** Support saving, sharing, and RSVPing to experiences.

### User Stories:
- **US-5.1**: As a user, I want to favorite events to view later.
- **US-5.2**: As a user, I want to RSVP to events directly or via external links.
- **US-5.3**: As a user, I want to leave a 1–5 star rating and optional feedback after attending an event.
- **US-5.4**: As a user, I want to share event links via text or social media.

---

## 📊 EPIC 6: AI Feedback & Analytics

**Goal:** Improve recommendations using engagement feedback.

### User Stories:
- **US-6.1**: As a system, I want to log when a recommendation is shown and clicked.
- **US-6.2**: As a system, I want to store recommendation context (mood, time, weather).
- **US-6.3**: As a user, I want to optionally see why something was recommended (explainable AI).

---

## 📱 EPIC 7: Mobile-First UX/UI

**Goal:** Deliver an intuitive, responsive, and visually appealing mobile experience.

### User Stories:
- **US-7.1**: As a user, I want a mobile-optimized interface with card-style event previews.
- **US-7.2**: As a user, I want a map-based discovery view with event pins.
- **US-7.3**: As a user, I want a floating filter widget to easily refine my search.
- **US-7.4**: As a user, I want a dark mode option.

---

## 🔐 EPIC 8: Authentication & Security

**Goal:** Secure user access and data.

### User Stories:
- **US-8.1**: As a user, I want my login credentials to be securely stored.
- **US-8.2**: As a developer, I want to enforce OAuth and Google/Facebook login.
- **US-8.3**: As a system, I want to restrict sensitive actions to authenticated users only.

---

## 🔄 EPIC 9: Admin & Content Dashboard

**Goal:** Support internal moderation and analytics.

### User Stories:
- **US-9.1**: As an admin, I want to approve/edit submitted events before they go live.
- **US-9.2**: As an admin, I want to track engagement metrics and user feedback in a dashboard.
- **US-9.3**: As an admin, I want to flag or remove abusive user submissions or feedback.

---

## ⏱ Suggested Implementation Milestones

| Phase    | Epics Involved             | Duration |
|----------|----------------------------|----------|
| Phase 1  | 1, 2, 4, 7                 | 3 weeks  |
| Phase 2  | 3, 5, 6                    | 4 weeks  |
| Phase 3  | 8, 9 + QA + UX Polish      | 2 weeks  |

---

