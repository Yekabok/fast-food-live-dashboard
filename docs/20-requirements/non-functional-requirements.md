# Non-Functional Requirements

## 1. Performance
### NFR-1.1 Dashboard load speed
The public dashboard should load quickly enough to support in-the-moment decision-making, especially on mobile connections.

### NFR-1.2 Interaction responsiveness
Changing area, sorting, or changing time window should update the interface with minimal perceived delay.

## 2. Availability and Reliability
### NFR-2.1 Service availability
The platform should be available at a level appropriate for a public consumer-facing service with frequent short visits.

### NFR-2.2 Data reliability
The system should avoid displaying stale or misleading live data without clearly indicating freshness or limited confidence.

## 3. Scalability
### NFR-3.1 Growth in users and submissions
The platform should be able to scale to support growth in public traffic, authenticated users, and rating submissions.

### NFR-3.2 Growth in historical data
The data model should support accumulation of historical ratings for later analytics without degrading core dashboard performance.

## 4. Security
### NFR-4.1 Secure authentication
Authentication shall rely on secure third-party identity providers and industry-standard session handling.

### NFR-4.2 Personal data protection
Personal information, including account data and contribution history, shall be stored and transmitted securely.

### NFR-4.3 Abuse resistance
The platform should include reasonable protections against spam, automated abuse, duplicate submissions, and manipulation of public scores.

## 5. Privacy and Compliance
### NFR-5.1 Privacy Act alignment
The platform shall support compliance with New Zealand privacy obligations relating to collection, notice, storage, access, correction, retention, and breach response.

### NFR-5.2 Consent and messaging controls
If the platform sends account or marketing communications, it shall support consent management and appropriate unsubscribe mechanisms where required.

### NFR-5.3 Cross-border data awareness
The system design should account for any overseas storage, authentication, or processing of personal data.

## 6. Usability
### NFR-6.1 Mobile-first usability
The primary experience shall be optimised for mobile devices.

### NFR-6.2 Scanability
The dashboard shall present comparative information in a way that can be understood quickly with minimal reading.

### NFR-6.3 Low-friction contribution flow
The rating submission process should be fast and simple enough to encourage repeat participation.

## 7. Accessibility
### NFR-7.1 Accessible visual communication
The platform should not rely on colour alone to communicate score states or confidence.

### NFR-7.2 Inclusive interaction
Core flows such as browsing, signing in, and rating should be operable with common accessibility needs in mind.

## 8. Transparency and Trust
### NFR-8.1 Explainability
The platform should clearly explain the meaning of gauges, confidence indicators, and time windows.

### NFR-8.2 Honest representation
The interface should avoid implying a level of precision or certainty that the underlying crowd-sourced data cannot support.

## 9. Maintainability
### NFR-9.1 Modular evolution
The system should be structured so live dashboard functionality, user accounts, scoring logic, and historical analytics can evolve independently.

### NFR-9.2 Configurability
Administrators should be able to adjust key operational settings such as time-window options, confidence thresholds, and store metadata without major redevelopment.

## 10. Observability
### NFR-10.1 Operational monitoring
The system should support monitoring of application health, submission activity, and abnormal behaviour.

### NFR-10.2 Auditability
The platform should retain enough submission and processing history to investigate disputes, anomalies, or abuse in internal operations.
