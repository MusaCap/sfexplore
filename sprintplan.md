# 🏁 ExploreSF Sprint Plan (Windsurf MVP Launch)

**Start Date:** TBD  
**Sprint Length:** 2 weeks  
**Total Sprints:** 4 (plus 1 optional polish sprint)  
**Team:** 1 PM, 1 UI/UX, 2 Frontend, 1 Backend, 1 AI Engineer

---

## 🧱 Sprint 1: Foundation Setup & Core Discovery

**Focus:** User onboarding, filtering engine, and event discovery.

### Goals:
- Implement user registration and preferences system.
- Build search and filter interfaces.
- Integrate location and category filters.

### Stories:
- US-1.1: Email or social sign-up
- US-1.2: Set age, location, mood
- US-1.3: Select interests on onboarding
- US-2.1: Freeform event search
- US-2.2: Filtering by category, vibe, cost, etc.
- US-2.5: Event detail view
- US-1.5: Auto-detect location

### Deliverables:
- Working onboarding flow
- Basic event discovery UI
- Functional filters and sorting

---

## 🌍 Sprint 2: External Data Integrations & Event Cards

**Focus:** API ingestion + data model + mobile-friendly UI.

### Goals:
- Ingest live event/venue data.
- Build responsive card-based UI.
- Display map-based results.

### Stories:
- US-4.1: Eventbrite API integration
- US-4.2: Yelp venue integration
- US-4.3: SF Funcheap RSS parser
- US-2.3: Map/list views
- US-7.1: Mobile card-style preview
- US-7.2: Map view of events

### Deliverables:
- Daily-synced event database
- Mobile-responsive views
- Venue/event detail linking

---

## 🤖 Sprint 3: AI Recommendation Engine & Interactions

**Focus:** AI personalization & engagement tracking.

### Goals:
- Launch core recommendation system.
- Build feedback loop for event choices.
- Enable favoriting and RSVP.

### Stories:
- US-3.1: Personalized event recs
- US-3.2: Mood-based suggestions
- US-3.4: Time/weather-based recs
- US-5.1: Favorite events
- US-5.2: RSVP to events
- US-6.1: Log rec impressions/clicks
- US-6.2: Context-aware tracking

### Deliverables:
- MVP recommender with GPT/embedding
- Actionable cards (RSVP, Save)
- Behavior log for analytics

---

## 🔐 Sprint 4: Admin Tools, Security, and Launch Polish

**Focus:** Admin dashboard, auth, and final QA.

### Goals:
- Secure app endpoints and enforce login.
- Add moderation and basic metrics.
- Run full QA with design polish.

### Stories:
- US-8.1: Secure credential handling
- US-8.2: OAuth & social login
- US-9.1: Admin event approval
- US-9.2: Feedback & metrics dashboard
- US-7.3: Floating filter widget
- US-7.4: Dark mode toggle

### Deliverables:
- Admin dashboard
- Hardened auth flows
- Production-ready interface

---

## 🎨 Optional Sprint 5: UX Polish & Social Sharing

**Focus:** Delight features, growth, and visual refinements.

### Goals:
- Add “Surprise Me” and “Explain this rec” features.
- Support social sharing + event viral loops.

### Stories:
- US-3.3: "Surprise Me" itinerary
- US-6.3: Explainable AI recs
- US-5.4: Social media share
- US-9.3: Flag/remove content
- Optional: Add GPT-powered chatbot planner

### Deliverables:
- AI polish features
- Shareable event experiences
- GPT planning assistant (beta)

---

## 🧭 Deployment Milestones

| Sprint | Duration     | Outcome                            |
|--------|--------------|-------------------------------------|
| 1      | Week 1–2     | Core onboarding + discovery UI      |
| 2      | Week 3–4     | Live event data + map integration   |
| 3      | Week 5–6     | Recs + RSVP/save logic              |
| 4      | Week 7–8     | Auth, admin, dark mode + QA         |
| 5★     | Week 9–10    | Social, polish, and explainable AI  |

---

**Notes:**
- Use Windsurf agents to scaffold each Epic as a project with code agents, UI agents, and integration agents.
- Stories can be tagged by EPIC ID and prioritized within the Windsurf backlog dashboard.

