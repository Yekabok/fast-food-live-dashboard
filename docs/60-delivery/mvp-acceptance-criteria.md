# MVP Acceptance Criteria

## 1. Public dashboard
- A public user can open the site and view a dashboard of stores for a selected area.
- Each visible store row includes the store icon, name, four gauges, confidence indicator, and last updated timestamp.
- The dashboard supports a default 15-minute time window.
- The user can change the active time window.

## 2. Comparative usability
- A user can compare multiple stores without opening a detail page.
- A user can distinguish between stronger and weaker live signals.
- A user can identify when a store has limited recent data.

## 3. Authentication
- A user can sign in successfully with Google.
- A user can sign in successfully with Apple.
- A signed-in session correctly associates the user with a verified email identity.

## 4. Rating submission
- A signed-in user can select a store.
- A signed-in user can submit structured ratings for service, speed, freshness, and order accuracy.
- A successful submission is stored and reflected in the system.

## 5. User profile
- A signed-in user can access a profile page.
- The profile page displays contribution count and earned badges.

## 6. Trust and interpretation
- A public user can access an explanation of score meaning, confidence, and time-window behaviour.
- The interface does not present low-confidence or stale data as if it were a strong live signal.

## 7. Operational readiness
- Administrators can maintain the store directory.
- Administrators can review or intervene in suspicious rating activity.
- The platform stores enough data to support future historical analytics.
