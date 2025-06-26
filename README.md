# Golden Pulse – Real-Time Accident Analysis and Emergency Response Optimization

Golden Pulse is an intelligent emergency response platform that revolutionizes accident reporting and resource allocation in real time. It minimizes delays in ambulance dispatch and hospital preparedness using machine learning, geospatial analysis, and accessible user interfaces like Telegram bots, Android apps, and web dashboards.

## Problem Statement

In India, thousands of lives are lost every year due to delayed emergency responses after road accidents. Current systems rely on slow, mediator-based processes with limited real-time visibility into ambulance or hospital availability. Golden Pulse addresses this challenge by integrating AI, NLP, and live communication to save time—and lives.

---

## Key Features

- **Multilingual Accident Reporting** via Telegram Bot using NLP for voice/text input
- **Clustering of Accident Zones** using DBSCAN
- **Live Ambulance Tracking** with real-time location updates and ETA calculation
- **Dynamic Hospital Suggestion** using KNN based on proximity and resource availability
- **Emergency Requirement Prediction** using XGBoost
- **Web Dashboard for Hospitals** with ambulance tracking and incident alerts
- **Bidirectional Real-Time Communication** using WebSockets
- **MongoDB-based Data Persistence** with geospatial indexing

---

## Tech Stack

| Component        | Technology                      |
|------------------|----------------------------------|
| Bot Interface    | Telegram, Python-Telegram-Bot   |
| Ambulance App    | Android, WebSocket Client       |
| Hospital Portal  | HTML, CSS, JS, Leaflet.js       |
| Backend Server   | Flask, Flask-SocketIO, REST API |
| Database         | MongoDB                         |
| ML Models        | DBSCAN, KNN, XGBoost            |
| Maps & Routing   | OSRM, Leaflet.js, Google Maps   |

---

## System Components

### 1. **Telegram Bot**
- Lightweight emergency reporting tool
- Supports voice commands and location sharing
- No app installation needed

### 2. **Ambulance Mobile App**
- Live alerts and routing
- Real-time patient status updates to hospitals
- Background GPS tracking

### 3. **Hospital Web Dashboard**
- Live map of ambulances en route
- Incident alerts with patient count/severity
- ICU/oxygen/staff availability management

### 4. **Backend Services**
- Built using Flask + MongoDB
- ML-based decision making for dispatch and hospital selection
- Real-time WebSocket communication between all components

---

## Machine Learning Modules

| Module            | Purpose                                       | Model     |
|-------------------|-----------------------------------------------|-----------|
| Accident Clustering | Identify accident hotspots                    | DBSCAN    |
| Resource Prediction | Estimate ambulance and ICU needs             | XGBoost   |
| Hospital Ranking    | Suggest best hospital based on real-time data | KNN       |

---

## Sample Results

| Metric                     | Value         |
|----------------------------|---------------|
| Clustering (Silhouette)    | 0.85          |
| XGBoost MAE                | 54.5          |
| Response Latency (avg.)    | < 1 second    |

---

## Data Flow

1. Public user reports accident via Telegram bot
2. System clusters the report, predicts needs, and locates nearest ambulance
3. Ambulance receives alert and shares live location during transit
4. Hospital receives ETA, patient details, and prepares resources
5. System logs events and enables analytics on response efficiency

---

## Future Enhancements

- ABHA health record integration
- Traffic-aware routing via Google Maps API
- Voice-based IVR system for elderly users
- AI-powered triage and predictive analysis

---

##  Authors

- **Sri Dharani R** – sridharanirajendran26@gmail.com  
- **Hemachandar K** – hemachandark333@gmail.com  
- **Jeyabalan P** – jeyabalan764@gmail.com

---

## Acknowledgments

We extend our gratitude to our mentors and institutions for their support, and to all open-source developers whose work helped make this project possible.

