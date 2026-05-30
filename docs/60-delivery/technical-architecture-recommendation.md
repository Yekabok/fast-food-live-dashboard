# Technical Architecture Recommendation

## Architectural goals
- fast public dashboard delivery
- simple structured contribution flow
- explainable live aggregation
- support for future historical analytics
- secure third-party authentication
- maintainable evolution from MVP to broader platform

## Recommended MVP architecture style
A modern web application with:
- server-rendered or hybrid-rendered frontend for fast initial load
- backend application layer for auth, data access, and aggregation
- relational database for core structured entities
- scheduled or on-demand aggregation layer for live and historical summaries

## Suggested logical components
### 1. Frontend
Responsibilities:
- dashboard rendering
- area selection
- sorting and time-window controls
- auth entry points
- rating submission UI
- profile pages
- trends views

### 2. Backend API or application layer
Responsibilities:
- store lookup
- rating ingestion
- authentication callbacks
- live signal calculation
- confidence calculation
- badge assignment
- admin tooling endpoints

### 3. Database
Responsibilities:
- store data
- user data
- raw rating submissions
- derived live signals
- badge state
- historical aggregates
- moderation metadata

### 4. Background processing
Responsibilities:
- recalculating live aggregates
- generating historical summaries
- detecting suspicious activity patterns
- running maintenance or cleanup jobs

## Data strategy recommendation
- store raw rating submissions permanently or for a long enough period to support audit and recalculation
- derive live dashboard signals from raw submission data
- precompute historical aggregates for longer reporting windows
- keep confidence as an explicit computed field

## Security and compliance considerations
- use trusted OAuth providers for sign-in
- minimise personal data collection
- secure stored user data and auth tokens
- log important actions for auditability
- design for privacy notice and future user-data access workflows

## Build recommendation
Use an architecture that keeps the public dashboard, contribution flow, and aggregation logic cleanly separated. This will make it easier to refine scoring and confidence models without rewriting the whole product.
