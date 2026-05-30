# Functional Requirements

## 1. Public Store Discovery
### FR-1.1 Area selection
The system shall allow users to view stores in a selected local area.

### FR-1.2 Location input
The system shall support area selection through one or more of the following methods:
- device location
- manual area search
- selectable list or map interface

### FR-1.3 Store listing
The system shall display a list of stores relevant to the selected area.

## 2. Public Dashboard
### FR-2.1 Dashboard row layout
For each store, the dashboard shall display:
- store icon
- store name
- service gauge
- speed gauge
- freshness gauge
- order accuracy gauge
- confidence indicator
- last updated timestamp

### FR-2.2 Comparative scanning
The dashboard shall allow users to compare multiple stores at a glance without needing to open a separate detail page.

### FR-2.3 Sorting
The dashboard should support sorting by:
- overall current score
- specific metric score
- confidence level
- most recently updated

### FR-2.4 Limited-data state
The dashboard shall visually distinguish stores with insufficient recent data.

## 3. Metric Visualisation
### FR-3.1 Gauge display
Each metric shall be displayed as a gauge with a neutral midpoint representing average performance.

### FR-3.2 Gauge direction
The gauge shall move in a negative direction for below-average recent feedback and in a positive direction for above-average recent feedback.

### FR-3.3 Gauge colour behaviour
The gauge shall change colour according to rating position, using an intuitive negative-to-positive colour spectrum.

## 4. Time Window Control
### FR-4.1 Default time window
The default dashboard scoring window shall be 15 minutes.

### FR-4.2 Configurable time window
The system shall allow users to change the time window used for score calculation.

### FR-4.3 Time-based aggregation
Only ratings within the currently selected time window shall contribute to the displayed live score.

## 5. Confidence and Freshness
### FR-5.1 Confidence display
The system shall display a confidence indicator for each store.

### FR-5.2 Confidence inputs
Confidence shall be based on the amount and recency of feedback in the active time window.

### FR-5.3 Update visibility
The system shall display the last updated timestamp for each store signal.

## 6. Authentication and Identity
### FR-6.1 Sign-in methods
Users shall be able to authenticate using:
- Google
- Apple

### FR-6.2 Verified account identifier
The system shall use the verified email provided by the identity provider as the primary account identifier.

## 7. Rating Submission
### FR-7.1 Store selection for rating
Authenticated users shall be able to select a store they have recently visited.

### FR-7.2 Structured rating submission
Authenticated users shall be able to submit ratings for:
- service
- speed
- freshness
- order accuracy

### FR-7.3 Submission confirmation
The system shall confirm successful submission of a rating.

### FR-7.4 Contribution rules
The system should enforce contribution limits or validation rules to reduce spam, duplication, or abuse.

## 8. User Profile and Contribution Recognition
### FR-8.1 User profile
Authenticated users shall have a profile page.

### FR-8.2 Profile content
The user profile shall display:
- display name
- contribution count
- earned badges
- recent activity summary

### FR-8.3 Badge system
The system should award badges or similar recognition based on user contribution milestones.

## 9. Historical Analytics
### FR-9.1 Trend views
The system should support historical performance views for periods such as:
- last week
- last month
- last 3 months
- last 6 months
- last 12 months

### FR-9.2 Historical comparison
The system should enable users to review how store performance changes over time.

## 10. Administration and Governance
### FR-10.1 Store data management
The system should support administration of the store directory and related metadata.

### FR-10.2 Abuse management
The system should support administrative actions to detect, review, and respond to suspicious or abusive rating activity.

### FR-10.3 Methodology transparency
The system should provide an accessible explanation of how scores, confidence, and time windows work.
