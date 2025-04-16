# 🌐 Emergency Alerts Application – Deliverable 1  
**Project Introduction & Scope Definition** 

---

## 1.1 Project Title  
**Emergency Alerts Application – Real-Time Crisis Notification System** 

---

## 1.2 Project Description  
A **mobile-first** platform delivering hyper-local emergency alerts via GPS and push notifications. 

### **Key Features**  
| Feature | Description | 

|---------|-------------|
 
| Real-Time Alerts | Push notifications for disasters, weather, and public safety threats. | 
| Geofencing | Alerts triggered only for users in affected zones (≤5km radius). | 
| Two-Way Reports | Users submit incidents (photos + GPS) for admin review. | 
| Historical Data | Exportable archive for trend analysis (CSV/PDF). | 

### **Supported Emergency Types**  
- **Natural Disasters**: Earthquakes, wildfires, floods. 
- **Weather Events**: Hurricanes, tornadoes, extreme heat. 
- **Public Safety**: Terrorist activity, chemical spills. 
- **Traffic**: Accidents, road closures. 

---

## 1.3 Key Objectives & Metrics  
| Objective | Success Metric | Tools/APIs | 

|-----------|---------------|------------|
 
| Geolocation Accuracy | ≤100m radius | Google Maps API, `react-native-geolocation` | 
| Alert Delivery Time | <5 seconds | Firebase Cloud Messaging (FCM) | 
| System Uptime | ≥99.9% SLA | Firebase Hosting, Load Balancing | 
| Concurrent Users | 10,000+ during surges | Kubernetes auto-scaling | 

---

## 1.4 Stakeholder Analysis  
| Stakeholder | Needs | Pain Points Addressed |
 
|-------------|-------|-----------------------| 

| **Citizens** | Instant, accurate alerts | Delayed/irrelevant warnings | 
| **Government** | Centralized alert distribution | Fragmented communication channels | 
| **First Responders** | Real-time incident clustering | Slow response times | 
| **Developers** | Scalable APIs, clear docs | Technical debt, poor logging | 

---

## 1.5 Constraints  
| Constraint | Mitigation Strategy | 

|------------|--------------------| 

| Poor network conditions | Offline-first design (Firestore cache) | 
| GDPR/CCPA compliance | Anonymize location data, user consent flows | 
| iOS/Android only | React Native for cross-platform support | 

---

## 1.6 Assumptions & Dependencies  
### **Assumptions**  
1. Users grant location permissions on app launch. 
2. Authorities verify alerts before publishing (admin dashboard). 
3. Public APIs (NOAA, USGS) provide reliable real-time data. 

### **Dependencies**  
| Dependency | Purpose | 

|------------|---------| 

| Firebase Authentication | User sign-up/login | 
| Google Maps API | Geofencing and map visualization | 
| Twilio (fallback) | SMS alerts if FCM fails | 

---
