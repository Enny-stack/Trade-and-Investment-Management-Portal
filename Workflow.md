# PRD — Trade & Investment Management Portal (TIMP)

## 1. Background / Problem
Business development roadshows and investment forums are high-impact, but today are constrained by manual operations, fragmented data, and inconsistent post-event follow-up. TIMP provides a single system to plan events, manage participant data securely, and convert engagement into structured transaction pipelines.

## 2. Objectives
1. Reduce operational burden of event execution (invitations, RSVPs, logistics).
2. Centralize stakeholder and investor data in a governed repository.
3. Provide a structured Deal Room that converts participation into actionable follow-up and measurable outcomes.
4. Provide analytics dashboards to track engagement and pipeline conversion.
5. Ensure secure, compliant data handling (GDPR-aligned; controlled access to sensitive materials).

## 3. Users & Roles
### Internal
- Admin users (COEV/TFIP/CLRE/Regional Staff/Digital Business): publish events, approve registrations, upload materials, moderate Deal Room activities, view analytics.
### External
- Verified users (investors, project owners, partners): register, access permitted materials, browse opportunities, request prospectus, schedule 1:1 meetings.

## 4. MVP Scope
**MVP modules**
- Event Management Suite (calendar, event profiles, registration)
- Deal Room (matchmaking-lite + meeting scheduling + “request prospectus”)
- Digital Deal Book (export workflow / PDF placeholder)
- Analytics (attendance, engagement, downloads)
- CRM sync (stub integration; define interface)

## 5. Functional Requirements (MVP)
### Event Management
- Admin creates event (venue, date, theme, banner, programme upload)
- Public event listing (calendar)
- Invitations and registration form (Name, Organisation, Title)
- Instant confirmation email + automated notification when materials are published
- Feedback surveys (ratings + comments)

### Deal Room
- Deal listing with filters: country, sector, ticket size
- Deal detail page: summary, key metrics, attachments/secure links, optional video link
- Actions: request prospectus; schedule 1:1 meeting (virtual or physical)
- Admin controls: publish/unpublish opportunities; verify readiness checklist for pitches

### Analytics
- Attendance metrics, engagement metrics (views/downloads), deal book downloads, meeting counts
- Export analytics for post-event reporting

### Security
- RBAC + secure data rooms for sensitive documents
- Audit-friendly activity logging (events, registrations, downloads, actions)

## 6. Non-Functional Requirements
- Multi-lingual UI: English, French, Arabic, Portuguese
- System segregation: Admin back-office vs Public front-end
- Regional segregation: North, East, West, Southern, Central, Caribbean
- Availability expectations for live events (basic DR approach)
- Privacy: minimization, encryption at rest/in transit, access logging

## 7. Success Metrics (MVP)
- % of invitees registering
- % of verified users accessing Deal Room
- # prospectus requests per event
- # 1:1 meetings scheduled per event
- Deal book downloads per event
- Post-event follow-up completion rate (actions closed within X days)

## 8. Dependencies / Integrations
- CRM: define read/write interface (contacts, engagement events, opportunity status)
- ATG ecosystem integration: Phase 2 but plan API surface

## 9. Open Questions (track as decisions)
- “Verified user” verification method (manual approval vs email domain vs invite token)
- Meeting scheduling integration (native calendar vs link-out)
- Document storage (SharePoint/OneDrive/S3-equivalent)
