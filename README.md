# 🚨 Emergency Alerts App

*Final Project – SENG8091: Software Engineering Principles*  
Developed by a team of two to create a scalable, secure, and real-time mobile application that notifies users of emergencies — such as weather hazards, public safety threats, or accidents — based on their geographic location or region of interest.

Author :- SHRIRANG RAVAL & MAHARSHI PUROHIT 

---

Instructor name :- ANDY CHOW

---

## 📖 Problem Statement

Many citizens do not receive critical emergency alerts in time due to fragmented notification systems, lack of personalization, and delayed delivery. Traditional systems like SMS, radio, or TV broadcasts are non-interactive, limited in reach, and not optimized for real-time user preferences.

This application aims to solve these problems by delivering:
- *Real-time alerts based on live location*
- *Push notifications for emergencies*
- *Interactive map views and historical alert tracking*
- *An intuitive mobile interface accessible to all age groups*

---

## 🧩 Project Objectives

- Create a mobile-first alert app with geolocation-based and manually filtered notifications.
- Ensure real-time delivery using Firebase Cloud Messaging.
- Enable verified authorities to issue alerts.
- Provide historical access to past incidents.
- Allow users to report nearby incidents (admin-verified).

---

## 📲 Key Features

### 👤 User Side
- *GPS-Based Alert Delivery*: Receive alerts relevant to current or selected regions.
- *Push Notifications*: Instant alerts on device using FCM (under 5 seconds).
- *Map Visualization*: View ongoing and past emergencies on a clustered map.
- *Filter & Search*: Find alerts by category, severity, region, or keywords.
- *Incident Reporting*: Submit photos, descriptions, and location data of events for admin review.
- *Alert History Archive*: Exportable logs of alerts (CSV, PDF) for future reference.

### 🛡️ Admin Side
- *Admin Dashboard*: Secure login with multi-factor authentication.
- *Alert Creation Tool*: Publish verified alerts with metadata (type, severity, region).
- *Moderation Queue*: Review and verify user-submitted reports before publishing.
- *Audit Logging*: Tracks all admin activity for traceability.

---

## 🧪 Functional & Non-Functional Requirements

See [Deliverable_2.md](./Deliverable_2.md) for full technical breakdown.

Highlights:
- ✅ Alerts delivered in < 5 seconds
- ✅ Location access with user consent
- ✅ Multi-factor authentication for admin dashboard
- ✅ Secure data handling (encrypted at rest and in transit)
- ✅ WCAG 2.1 compliant design for accessibility

---

## 📐 Task Breakdown & User Stories

Tasks were broken down into functional modules with agile methodology. See [Deliverable_3.md](./Deliverable_3.md) or [PHASE3.md](./PHASE3.md) for full user stories, acceptance criteria, and task tracking.

Key Modules:
- Location-based alerts
- Admin dashboard
- Push notification system
- Map-based visualizations
- Report submission
- Archive and filtering

---

## 🏗️ Technology Stack

| Layer              | Technology                                |
|--------------------|--------------------------------------------|
| *Frontend*       | React Native (Android & iOS Support)       |
| *Backend*        | Node.js with Express.js                    |
| *Database*       | Firebase Firestore                         |
| *Authentication* | Firebase Authentication (MFA enabled)      |
| *Notifications*  | Firebase Cloud Messaging (FCM)             |
| *Maps*           | Google Maps API                            |
| *Hosting*        | Firebase Hosting                           |
| *CI/CD*          | GitHub Actions                             |

---


