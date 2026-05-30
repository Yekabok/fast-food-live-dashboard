# Website Requirements Specification v1

## 1. Purpose
The website will provide the public with near real-time visibility into the recent customer-rated performance of fast food stores in their area.

## 2. Product goals
- Help users compare nearby stores quickly
- Surface current operating sentiment rather than long-term review averages
- Encourage frequent user contributions to maintain data freshness
- Support future trend analytics using historical rating data

## 3. Primary users
### 3.1 Public viewers
Users who want to assess which nearby fast food store is likely to provide the best current experience.

### 3.2 Registered contributors
Users who sign in and submit ratings based on a recent visit.

## 4. Core dashboard requirements
Each store row shall display:
- store icon
- store name
- gauge for service
- gauge for speed
- gauge for freshness
- gauge for order accuracy
- confidence rating
- last updated timestamp

## 5. Gauge behaviour
Each gauge shall:
- have a neutral midpoint representing average performance
- move in a negative direction for worse recent feedback
- move in a positive direction for better recent feedback
- change colour based on sentiment position

Suggested colour progression:
- poor: red
- below average: amber
- average: neutral grey or blue
- above average: green
- excellent: strong green

## 6. Time window requirements
- default score window shall be 15 minutes
- users shall be able to change the dashboard time window
- scores shall be based only on ratings within the selected window
- stores with insufficient recent data should show a low-confidence or limited-signal state

## 7. Rating metrics
Authenticated users shall be able to rate:
- service
- speed
- freshness
- order accuracy

## 8. Confidence requirements
The system shall calculate a confidence rating based on:
- number of ratings in the selected time window
- recency of ratings
- optional future consistency weighting

## 9. Authentication requirements
Users shall be able to sign in using:
- Google
- Apple

The platform shall use the verified email returned by the identity provider as the account identifier.

## 10. Profile requirements
Each user shall have a profile page containing:
- display name
- contribution count
- earned badges
- recent activity summary

## 11. Future analytics
The platform should support historical analysis views for:
- last week
- last month
- last 3 months
- last 6 months
- last 12 months

## 12. Out of scope for MVP
- store owner portal
- dispute workflow for stores
- advanced business response tooling

## 13. Product recommendation
For MVP, prefer structured rating inputs over public free-text comments.
