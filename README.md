# AeroTracer — Aircraft Crash Prediction System

> **Bridging aviation data and predictive intelligence to enhance safety and accelerate emergency response.

---

## Overview

AeroTracer is an intelligent aviation safety platform designed to predict probable aircraft crash zones by integrating real-time and historical flight data with environmental and terrain variables. The system leverages supervised machine learning techniques on key parameters such as altitude, airspeed, weather conditions, fuel status, and terrain topology to generate accurate risk assessments. This enables aviation authorities and emergency response teams to make faster, data-driven decisions during critical situations.

A key differentiator of AeroTracer is its dedicated focus on radome-related failure analysis. Unlike conventional flight-tracking systems, AeroTracer investigates potential hardware anomalies—particularly radome degradation or damage—and examines their correlation with increased crash risk. This deeper analytical capability enhances predictive accuracy and contributes to improved aviation safety outcomes.

---

## Objectives

- Predict probable crash zones using live and historical flight parameters
- Perform real-time risk assessment across multiple aviation variables
- Reduce emergency response time through actionable predictive insights
- Advance aviation safety standards through data-driven analysis

---

## Key Features

| Feature | Description |
|---|---|
| 📡 Real-Time Flight Integration | Live flight data ingestion via the OpenSky Network API |
| 🌦️ Weather Analysis | Environmental factor modeling including wind, visibility, and precipitation |
| 🗺️ Terrain Modeling | Crash zone prediction accounting for topographic risk factors |
| 🤖 ML-Based Risk Engine | Supervised learning models for classification and regression tasks |
| 📊 Visualization Dashboard | Interactive crash zone mapping and insight analytics |
| 🔬 Radome Failure Research | Focused analysis of radome anomalies as a contributing crash factor |

---

## System Architecture

```
┌──────────────────────────────────────────────────────┐
│                   Data Collection Layer               │
│        OpenSky API · Weather APIs · Terrain Datasets  │
└────────────────────────┬─────────────────────────────┘
                         │
┌────────────────────────▼─────────────────────────────┐
│                  Data Processing Layer                │
│          Cleaning · Preprocessing · Feature Extraction │
└────────────────────────┬─────────────────────────────┘
                         │
┌────────────────────────▼─────────────────────────────┐
│                     Model Layer                       │
│    ML Models (Regression · Classification) · Engine   │
└────────────────────────┬─────────────────────────────┘
                         │
┌────────────────────────▼─────────────────────────────┐
│                  Visualization Layer                  │
│           Crash Zone Mapping · Analytics Dashboard    │
└──────────────────────────────────────────────────────┘
```

---

## Technology Stack

### Frontend
- HTML5 · CSS3 · JavaScript (ES6+)
- React *(planned enhancement)*

### Backend
- Node.js
- Express.js

### Machine Learning
- Python 3.x
- Scikit-learn · Pandas · NumPy

### APIs & Data Sources
- [OpenSky Network API](https://opensky-network.org/) — Real-time and historical flight data
- Weather API *(e.g., OpenWeatherMap / NOAA)* — Environmental conditions

---

## Machine Learning Approach

AeroTracer employs **supervised learning** to predict crash risk scores and probable impact zones. Models are trained on labeled aviation incident data combined with environmental readings.

### Input Features

| Parameter | Description |
|---|---|
| Altitude | Current flight level (ft/m) |
| Airspeed | Velocity vector (knots) |
| Weather Conditions | Wind, visibility, precipitation intensity |
| Fuel Status | Remaining fuel as a percentage of capacity |
| Terrain Type | Surface classification beneath the flight path |

### Models Under Evaluation

- **Logistic Regression** — Baseline binary risk classifier
- **Decision Trees** — Interpretable multi-class crash zone prediction
- **Random Forest** — Ensemble model for improved accuracy and robustness

---

## Research Focus: Radome Failure Analysis

A core research component of AeroTracer investigates **radome-related anomalies** — disruptions or failures in the protective nose cone housing an aircraft's weather radar. This research examines:

- Frequency and conditions of radome failures in historical incident data
- Correlation between radome degradation and navigational/weather radar inaccuracies
- Contribution of radome failures to crash probability scoring within the ML pipeline

This focused analysis aims to provide aviation safety regulators with actionable insight into an often-overlooked hardware risk factor.

---

## Getting Started

### Prerequisites

- Node.js (v16+)
- Python 3.8+
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/aerotracer.git

# Navigate to the project directory
cd aerotracer

# Install Node.js dependencies
npm install

# Install Python dependencies
pip install -r requirements.txt

# Start the backend server
npm start
```

The application will be available at `http://localhost:3000` by default.

---

> *AeroTracer — Predictive intelligence for a safer sky.*
