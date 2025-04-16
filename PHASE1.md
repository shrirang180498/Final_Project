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
