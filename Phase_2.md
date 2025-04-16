# 🚨 Final Project – Emergency Alerts App

## 📘 Deliverable 2: Functional & Non-Functional Requirements

---

## 2.1 Functional Requirements

The Emergency Alerts mobile application is intended to serve as a real-time public safety tool that notifies users of critical emergencies such as severe weather, accidents, or natural disasters. Below is a breakdown of its functional requirements:

---

### 🔐 1. User Registration and Login

- Users must be able to sign up and log in securely using Firebase Authentication.
- Supports email/password and OAuth (Google).
- Includes features like password recovery, validation, and session timeout.
- All sessions should be securely managed to prevent unauthorized access.

---

### 📍 2. Location Permissions for Region-Based Alerts

- The app should request and manage live location permissions from the user.
- Uses GPS coordinates and geofencing for accurate, region-specific alerts.
- Must also support background location tracking for continuous monitoring.

---

### 🚀 3. Push Notification Engine (Real-Time Alerts)

- Firebase Cloud Messaging (FCM) will be used to deliver instant alerts.
- Notifications must contain alert type, severity, region, and time metadata.
- Supports foreground and background delivery with click-to-open actions.

---

### 🛡️ 4. Admin Dashboard for Verified Institutions

- A secure web dashboard for government or institutional admins to publish alerts.
- Implements role-based access controls and audit logs for accountability.
- Only verified admins can manage public-facing alert content.

---

### ✍️ 5. Create/Edit/Delete Alerts with Metadata Tagging

- Admins can create alerts and assign metadata:
  - Alert type (e.g., fire, storm)
  - Severity level
  - Affected region (geolocation)
  - Timestamp and validity duration
  - Optional contact details or resources

---

### 🗺️ 6. Map Interface Showing Clustered Alerts

- Alerts will be shown on a dynamic map using Google Maps API.
- Supports clustering of alerts by region and zoom level.
- Users can tap map pins to read full alert information.

---


### 🎚️ 7. Alert Filtering Based on Type, Severity, Region, and Date

- Filters allow users to customize the view of alerts:
  - Type (e.g., accident, flood)
  - Severity (e.g., high, medium, low)
  - Region/geolocation
  - Date/time of occurrence

---

### 🗃️ 8. Historical Alert Archive with Search and Export

- Alerts will be archived and searchable by type, keyword, and date.
- Users can export alert data in CSV or JSON format for review or reporting.

---

### 🧾 9. Report Incident Feature (with Admin Review)

- Users can submit emergency reports via a structured form.
- Reports include text, optional images/videos, and location.
- All user-submitted reports must be reviewed and approved by admins.

---




## ✅ 2.2 Non-Functional Requirements

These characteristics define how the system will perform under various conditions and user expectations.

---

### ⚡ Performance

- Alerts must be pushed to users within 5 seconds of publishing.
- Interface responses must occur in under 1 second for core interactions.

---

### 📶 Availability

- The system must maintain ≥ 99.9% uptime during all operational periods.
- Auto-scaling and redundancy required to handle traffic surges during emergencies.

---

### 🔐 Security:

- Role-based access control for users and admins.
- Multi-Factor Authentication (MFA) required for admin dashboard access.
- Data must be encrypted at rest and in transit, ensuring compliance with data privacy laws.

---

### ⚙️ Scalability

- System must support more than 10,000 concurrent users.
- Backend and notifications must scale horizontally using cloud services.

---

### ♿ Accessibility

- UI/UX will follow WCAG 2.1 accessibility standards.
- Screen readers, contrast options, and navigation aids will be included.

---
