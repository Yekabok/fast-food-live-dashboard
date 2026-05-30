# Decision Log and Open Questions

## Confirmed decisions

### D-001
The product will focus on near real-time customer-rated fast food store performance.

### D-002
The core live dashboard metrics are:
- service
- speed
- freshness
- order accuracy

### D-003
The dashboard will use gauge-style visual indicators with a neutral midpoint.

### D-004
The dashboard will show a confidence indicator based on recent feedback volume and recency.

### D-005
The default live scoring window will be 15 minutes.

### D-006
Users will authenticate using Google or Apple.

### D-007
Users will have profile pages with contribution badges.

### D-008
The product will support historical analytics in a later phase.

### D-009
There will be no store owner portal or dispute workflow in the initial concept.

## Open questions

### Q-001 Store discovery
How exactly should users define or detect their area?
- device location
- suburb search
- postcode search
- map interaction

### Q-002 Store source data
What is the source of truth for the store directory?
- curated internal data
- third-party places data
- chain-by-chain onboarding

### Q-003 Contribution limits
How often can one user rate the same store?
- once per visit
- once per hour
- once per active time window

### Q-004 Rating eligibility controls
Should the system require additional proof or signal that the user was genuinely at the store?

### Q-005 Free-text comments
Will the MVP allow comments, or remain structured-rating only?

### Q-006 Profile visibility
What information on a user profile is public versus private?

### Q-007 Scoring methodology
What exact formula should convert raw ratings into gauge position and confidence?

### Q-008 Threshold behaviour
What should the platform show when recent feedback volume is too low?

### Q-009 Brand/store representation
Should rows represent branded locations only, or any quick-service restaurant?
