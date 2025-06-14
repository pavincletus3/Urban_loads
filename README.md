# 🔋 UrbanLoad

<div align="center">

![UrbanLoad Banner](https://img.shields.io/badge/UrbanLoad-Weather--Aware%20Energy%20Forecasting-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Hackathon](https://img.shields.io/badge/Hackathon-Hackera'25-orange)

_A Weather-Aware Urban Energy Load Forecasting System_

</div>

## 📝 Overview

UrbanLoad is a sophisticated web application that leverages weather data and machine learning to predict urban electricity demand. Built with sustainability in mind, it empowers users and urban planners with actionable insights aligned with UN SDG #7 (Affordable and Clean Energy).

🚀 Features
✅ AI-Driven Policy Engine – Converts forecast data into actionable energy insights for city planners.
📈 Weather-Aware Load Forecasting – Predicts energy demand based on temperature, humidity, and other environmental factors.
🔐 Role-Based Access with Clerk – Secure multi-user authentication and access control for analysts, admins, and general users.
🌍 Sustainability Insights – Estimates carbon footprint reduction from optimized energy usage.
📊 Interactive Dashboard – View city-wise load predictions, daily/hourly trends, and Power Usage visualizations.
🧠 Tech Stack
Layer Tech Used
ML Model Python, Jupyter Notebook (Trained on historical + weather data)
ML API Flask (serving predictions via REST API)
Backend Node.js (handles API routing, OpenWeather integration)
Frontend React.js (with Clerk for authentication)
Visualization Chart.js (for graphs and Graphs)
Hosting Vercel (Frontend), Railway/Render (Backend & Flask service)
🏗️ System Architecture
User selects a city and date range via React frontend.
Backend (Node.js) fetches weather forecast from OpenWeatherMap API.
Flask ML microservice predicts energy demand based on weather and historical patterns.
Results are displayed as graphs, charts and sustainability tips.
📂 Folder Structure
/Urbanapp → React Frontend
/Urban_Load → Node.js Backend API
/ml-service → Flask + Trained ML Model
README.md → You're here!
📊 Sample Inputs
City: Mumbai
Date Range: 2025-04-11 to 2025-04-13
Weather: 34°C, 70% humidity
Output: Predicted load in MW with CO₂ impact estimate
🛠️ Setup Instructions
Clone the repo

git clone https://github.com/your-username/smartgrid-ai.git
cd smartgrid-ai
Install dependencies

cd client && npm install # React
cd ../server && npm install # Node backend
cd ../ml-service && pip install -r requirements.txt # Flask service
Start services

# In separate terminals

cd client && npm start
cd server && node index.js
cd ml-service && python app.py
Create a Clerk project and add your frontend URL for authentication

Add OpenWeatherMap API key in your backend as an environment variable:

OPENWEATHER_API_KEY=your_key_here
🧪 Future Enhancements
Real-time data integration from smart meters
Geo-visual heatmaps with Leaflet.js
Admin analytics dashboard
Auto-policy recommendations for peak hours
🌱 Impact
By making urban energy load patterns predictable and visible, UrbanLoad empowers both individuals and city planners to:

Reduce peak-hour electricity consumption
Optimize energy infrastructure usage
Lower carbon emissions
Advance clean energy goals
Made with 💡 by Team Ctrl+Alt+Defeat(HAE-043) — Hackera'25 Submission
For queries or contributions, please contact: pavincletus123@gmail.com
