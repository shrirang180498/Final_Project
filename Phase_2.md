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

