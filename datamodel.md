# 📊 ExploreSF Data Model (Entity-Relationship Overview)

## 🧱 Core Entities

### 1. `User`
Stores basic user account information and preferences.

```sql
User (
  id UUID PRIMARY KEY,
  email VARCHAR(255) UNIQUE,
  name VARCHAR(100),
  location GEOGRAPHY(Point),
  age INT,
  gender VARCHAR(10),
  signup_method VARCHAR(50),
  created_at TIMESTAMP,
  updated_at TIMESTAMP
)
2. UserPreferences
Captures user interests, preferred categories, mood, etc.

sql
Copy
Edit
UserPreferences (
  id UUID PRIMARY KEY,
  user_id UUID REFERENCES User(id),
  categories TEXT[],          -- e.g. ['Art', 'Music', 'Food']
  tags TEXT[],                -- e.g. ['Afrofuturism', 'Jazz']
  preferred_budget_range INT[],
  typical_mood TEXT,          -- e.g. 'chill', 'adventurous'
  update_frequency VARCHAR(10),
  updated_at TIMESTAMP
)
Event (
  id UUID PRIMARY KEY,
  title VARCHAR(255),
  description TEXT,
  start_time TIMESTAMP,
  end_time TIMESTAMP,
  venue_id UUID REFERENCES Venue(id),
  category VARCHAR(50),            -- e.g. 'Nightlife', 'Wellness'
  tags TEXT[],
  cost_range INT,                  -- min price in dollars
  is_ticketed BOOLEAN,
  ticket_url TEXT,
  source VARCHAR(50),              -- e.g. 'Eventbrite', 'Manual'
  external_id VARCHAR(255),        -- ID from external system
  popularity_score FLOAT,
  image_url TEXT,
  created_at TIMESTAMP,
  updated_at TIMESTAMP
)
Venue (
  id UUID PRIMARY KEY,
  name VARCHAR(255),
  address TEXT,
  city VARCHAR(100),
  latitude FLOAT,
  longitude FLOAT,
  type VARCHAR(50),              -- e.g. 'Cafe', 'Gallery'
  description TEXT,
  yelp_rating FLOAT,
  website_url TEXT,
  created_at TIMESTAMP,
  updated_at TIMESTAMP
)
UserFavorites (
  id UUID PRIMARY KEY,
  user_id UUID REFERENCES User(id),
  event_id UUID REFERENCES Event(id),
  favorited_at TIMESTAMP
)
UserRSVP (
  id UUID PRIMARY KEY,
  user_id UUID REFERENCES User(id),
  event_id UUID REFERENCES Event(id),
  rsvp_status VARCHAR(10),    -- e.g. 'going', 'interested'
  rsvp_time TIMESTAMP
)
UserFeedback (
  id UUID PRIMARY KEY,
  user_id UUID REFERENCES User(id),
  event_id UUID REFERENCES Event(id),
  rating INT,                  -- 1–5 stars
  comment TEXT,
  submitted_at TIMESTAMP
)
RecommendationLog (
  id UUID PRIMARY KEY,
  user_id UUID REFERENCES User(id),
  event_id UUID REFERENCES Event(id),
  recommended_at TIMESTAMP,
  clicked BOOLEAN DEFAULT FALSE,
  context JSONB                 -- e.g. mood, weather, query string
)
Tag (
  id UUID PRIMARY KEY,
  name VARCHAR(50) UNIQUE
)
EventTag (
  id UUID PRIMARY KEY,
  event_id UUID REFERENCES Event(id),
  tag_id UUID REFERENCES Tag(id)
)
EventEmbedding (
  id UUID PRIMARY KEY,
  event_id UUID REFERENCES Event(id),
  embedding VECTOR(1536),  -- or float[] based on model
  model_version TEXT,
  created_at TIMESTAMP
)
