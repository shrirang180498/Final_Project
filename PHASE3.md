# ✅ Deliverable 3: Task Breakdown, User Stories, and Acceptance Criteria

This document outlines the actionable development tasks required to build the Emergency Alerts App. Each task includes a clearly defined user story and a detailed set of acceptance criteria, designed to guide implementation and testing.

---

## 🔧 Task 1: Location-Based Alert Subscription

### 🧑‍💼 User Story
*As a* user,  
*I want* to receive emergency alerts based on my current real-time location or a region I manually select,  
*So that* I stay informed about emergencies relevant to me, even when I’m on the move.

### ✅ Acceptance Criteria
- The app must request and obtain user permission for GPS access at launch or during setup.
- Users must have the option to manually select a region if GPS access is denied.
- The system must geofence alert zones and determine whether a user is inside the affected area.
- Alerts should be automatically refreshed and updated as the user’s location changes.
- Push notifications are delivered within 3 to 5 seconds of the alert being triggered by the admin.
- If location permissions are revoked, a fallback message must be shown informing the user to enable access.

---

## 🔧 Task 2: Alert Creation by Verified Admins

### 🧑‍💼 User Story
*As an* authorized administrator,  
*I want* to securely log in and create emergency alerts with all necessary details (location, type, severity, message),  
*So that* the public is notified quickly and efficiently during emergencies.

### ✅ Acceptance Criteria
- Admins must authenticate using Firebase Auth and Multi-Factor Authentication (MFA).
- Alert creation form includes fields for:
  - Alert Title
  - Type (Weather, Traffic, Crime, etc.)
  - Severity (Low, Medium, High)
  - Description
  - Affected Regions (single or multiple with map selection)
  - Duration (optional expiration timestamp)
- Preview option available before publishing.
- Upon publishing, alert is immediately visible on the map and pushed to users in the selected region.
- Alert publishing history is logged with admin ID, timestamp, and changes.

---

## 🔧 Task 3: Push Notification Engine Integration

### 🧑‍💻User Story
*As a* developer,  
*I want* to integrate Firebase Cloud Messaging (FCM) for real-time push notifications,  
*So that* users are promptly notified about emergencies without opening the app.

### ✅ Acceptance Criteria
- FCM service is initialized and configured in both the mobile frontend and backend.
- Notifications are automatically triggered when a new alert is published.
- Notification payload includes:
  - Title
  - Body (short description)
  - Alert type
  - Region identifier
  - Timestamp
- Delivery performance must be tested under load to ensure latency is < 5 seconds.
- Retry mechanism implemented to reattempt failed deliveries.
- User preferences must be respected—alerts must not be pushed if a category is disabled in their settings.

---

## 🔧 Task 4: Map-Based Visualization of Alerts

### 🧭 User Story
*As a* user,  
*I want* to see emergency alerts visually plotted on an interactive map,  
*So that* I can understand where incidents are happening in real-time and assess my proximity to them.

### ✅ Acceptance Criteria
- The map (powered by Google Maps API) is embedded within the app's dashboard.
- Active alerts are displayed as pins/icons with location-based clustering enabled.
- Tooltip or bottom-sheet appears when a pin is tapped, showing:
  - Alert type
  - Severity level (color coded)
  - Description
  - Time issued
- Alerts should be visually differentiated by severity:
  - Red = High
  - Orange = Medium
  - Yellow = Low
- User's current location is shown as a marker on the map.
- Alerts auto-refresh as new ones are created or old ones expire.
 
---


## 🔧 Task 5: Filter and Search Alerts

### 🧑‍💼 User Story
**As a** user,  
**I want** to filter and search through alerts by type, severity, region, and time,  
**So that** I can find the alerts that matter most to me quickly and efficiently.

### ✅ Acceptance Criteria
- Filter panel must include:
  - Alert Type (checkboxes)
  - Severity Level (dropdown or toggle)
  - Date Range Selector
  - Region (if not using GPS)
- A global search bar allows for keyword-based searching within alert titles and descriptions.
- Filter and search results update the map and alert list dynamically without requiring app reload.
- "Clear All" option resets filters to default.

---

