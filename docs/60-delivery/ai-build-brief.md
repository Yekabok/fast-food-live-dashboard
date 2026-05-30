# AI Build Brief

## Purpose
This document provides implementation context for an AI coding agent or development team building the Fast Food Live Dashboard product.

## Product summary
Build a public website that lets users view the recent customer-rated performance of nearby fast food stores and compare them in near real time. The product should prioritise recency, comparability, trust, and mobile usability.

## Core product behaviour
The system must:
- show fast food stores in a selected area
- present each store in a compact dashboard row
- display four live metrics: service, speed, freshness, order accuracy
- display a confidence indicator for each store
- display the last updated time for each store
- use a default score time window of 15 minutes
- allow the time window to be changed
- allow authenticated users to sign in with Google or Apple
- allow authenticated users to submit structured ratings
- provide user profiles with contribution counts and badges

## UX priorities
1. Make it easy to compare stores quickly.
2. Make low-confidence data obvious.
3. Make the dashboard usable on mobile first.
4. Keep contribution flows short and low friction.
5. Separate live dashboard behaviour from historical trends.

## MVP implementation priorities
### Priority 1
- project scaffolding
- store directory model
- area-based dashboard
- live score aggregation
- time-window filtering
- confidence display

### Priority 2
- authentication with Google and Apple
- structured rating submission flow
- user profile page
- basic badge system

### Priority 3
- historical aggregation support
- trends page
- admin moderation tools
- methodology explainer page

## Constraints and guidance
- Treat the dashboard as a crowd-sourced recent sentiment product, not an official operational measurement system.
- Avoid UI language that implies scientific certainty where the data may be sparse.
- Design the scoring model to be explainable.
- Keep the data model flexible enough to support later analytics.
- Assume anti-abuse controls are required, even if basic in MVP.

## Recommended implementation sequence
1. Define the data schema.
2. Build store listing and area selection.
3. Implement dashboard row and gauge components.
4. Build live score calculation logic.
5. Add confidence and freshness signals.
6. Add authentication.
7. Add contribution flow.
8. Add profile and badges.
9. Add historical aggregation hooks.
10. Add admin and governance tooling.

## References
See related documents in:
- `docs/20-requirements/`
- `docs/30-ux/`
- `docs/40-data/`
- `docs/50-compliance/`
- `docs/60-delivery/`
