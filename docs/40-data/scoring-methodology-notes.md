# Scoring Methodology Notes

## Objective
Translate raw structured ratings into live comparative signals that are easy to understand and quick to scan.

## Inputs
- service rating
- speed rating
- freshness rating
- order accuracy rating
- submission timestamp
- store identity
- user identity for validation and anti-abuse controls

## Key requirements for the methodology
- strongly favour recent submissions
- support configurable time windows
- remain understandable enough to explain to users
- avoid overreacting to a single submission where confidence is low
- allow low-volume situations to be represented honestly

## Candidate approach for MVP
- Use ratings within the active time window only.
- Calculate per-metric averages for the store.
- Map the average onto a gauge position around a neutral midpoint.
- Calculate confidence separately from score.
- Reduce visual certainty when the volume of data is low.

## Methodology concerns still to resolve
- minimum submission threshold for meaningful display
- whether newer submissions should be weighted more heavily inside the same time window
- whether contributor trust or historical behaviour should affect weighting
- how overall score should be derived from the four metrics
- how to handle conflicting recent submissions

## Recommendation
Keep the first live methodology simple, explainable, and transparent. Sophisticated weighting can be introduced later if needed.
