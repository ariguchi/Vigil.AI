# VigilAI
VigilAI is a real-time crime analysis and prediction system that detects patterns, connects possibly related crimes, and identifies emerging hotspots using data-driven intelligence.



## Problem Statement
Crime systems are reactive, not predictive → action starts after damage is done
Rising urban crime is worsened by delayed detection and manual analysis
Emerging hotspots go unnoticed until they escalate
No real-time intelligence → slow response, poor resource use
Dashboards show data, not connections → patterns stay hidden
Missed patterns today become crimes tomorrow



## Proposed Solution
Analyzes crime data as interconnected signals rather than isolated incidents
Detects key indicators: crime spikes, pattern clusters, and hotspot intensity
Identifies trends, emerging threats, and hidden connections in real time
Provides a dynamic, continuously updating view for faster and smarter decision-making



## Features
| Tab            | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| Weekly Spikes  | Z-score–based anomaly detection on weekly crime volumes                    |
| District Map   | Interactive Folium map with pulse-ring animations and "crime web" lines    |
| Breakdown      | Category, day-of-week, and hour-level crime breakdowns                     |
| Clusters       | KMeans geographical hotspot clustering                                     |
| Explainer      | Actionable intelligence panel with recommended patrol actions              |


- Crime hotspots represented as dynamic nodes (dots) Size = intensity of crime Green = Low Risk Yellow = Medium Risk Red = High Risk
- Pattern-based connections between similar crimes
- Web-like visualization on real geographic maps
- Identification of connected crime networks
- Real-time crime surge detection with pulse/vibration effect
- Alerts for nearby at-risk zones

## Setup

### 1) Clone the repo
```git clone https://github.com/ariguchi/VigilAI.git```
```cd VigilAI```

### 2) Install Dependencies
```pip install -r requirements.txt```

### 3) Add the dataset
```data/train.csv```

### 4) Run the app
```streamlit run app.py```
