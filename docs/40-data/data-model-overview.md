# Data Model Overview

## Core entities

## 1. Store
Represents a physical fast food location.

### Suggested attributes
- store_id
- brand_name
- store_name
- address
- suburb or locality
- region
- latitude
- longitude
- active status

## 2. User
Represents an authenticated contributor.

### Suggested attributes
- user_id
- email
- auth_provider
- display_name
- created_at
- badge_state
- contribution_count

## 3. Rating Submission
Represents one structured user contribution for a specific store and time.

### Suggested attributes
- rating_id
- user_id
- store_id
- submitted_at
- visit_time or rating_time
- service_score
- speed_score
- freshness_score
- order_accuracy_score
- source_metadata
- moderation_status

## 4. Live Store Signal
Represents the calculated live view of a store for a selected time window.

### Suggested attributes
- store_id
- time_window
- calculated_at
- service_signal
- speed_signal
- freshness_signal
- order_accuracy_signal
- overall_signal
- confidence_level
- rating_count
- last_submission_at

## 5. Badge
Represents a contribution recognition milestone.

### Suggested attributes
- badge_id
- badge_name
- badge_description
- threshold_rule

## 6. Historical Aggregate
Represents summary data for longer trend analysis.

### Suggested attributes
- store_id
- date_period
- metric_name
- average_score
- confidence_level
- submission_count

## Data design notes
- Live dashboard calculations should be derived from recent submission data rather than manually edited values.
- Historical reporting data may be pre-aggregated for performance.
- Moderation and auditability fields should be included to support abuse review.
- Confidence should be a first-class data concept, not only a visual label.
