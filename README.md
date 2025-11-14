🌱 IoT & AI-Enabled Precision Farming System
Real-Time Soil Monitoring | AI Crop Recommendation | Automated Alerts

This project is a smart precision farming solution built using Raspberry Pi 5, a 6-in-1 RS485 Soil Sensor, and AI-based crop analysis.
It helps farmers/gardeners monitor soil health, get intelligent crop suggestions, and receive timely alerts for nutrient imbalance.

🚀 Features

📡 Real-time Soil Data (Moisture, Temperature, pH, Nitrogen, Phosphorus, Potassium)

🧠 AI-Powered Crop Recommendations using Gemini API

🔍 Crop Suitability Check for any user-entered crop

📊 Live Dashboard built with Flask

📄 PDF Report Generation (Soil Report & AI Analysis Report)

🔔 Continuous Monitoring + Email Alerts when nutrient levels deviate

💬 Smart Gardening Chatbot

🔁 Automatic sensor polling every 30 seconds

🛠 Hardware Used

Raspberry Pi 5

RS485 Soil Sensor (6-in-1)

USB → RS485 Converter

5V 3A Power Supply

12V Adapter for sensor

💻 Tech Stack

Backend: Python, Flask
AI Engine: Gemini 2.5 Flash
Protocols: Modbus RTU (RS485)
PDF Engine: WeasyPrint
Email: SMTP

📂 Project Structure
/templates     → HTML files (Dashboard, Analysis, PDF views)
/static        → CSS, JS, Assets
app.py         → Main backend logic
.env           → API keys & SMTP credentials

🔧 Installation (Quick Setup)
pip install Flask minimalmodbus weasyprint python-dotenv google-generativeai


Start the server:

python3 app.py


Open in browser:

http://<your-pi-ip>:5001

📧 Email Alerts

System sends automated alerts when soil nutrient levels fall outside the ideal crop range
(One alert every 24 hours to avoid spamming).

📑 PDF Reports Generated

Soil Sensor Report

AI-Based Crop Recommendation Report

User Crop Suitability Report

All with timestamp, clean UI, and professional formatting.

📸 Screenshots

(Add screenshots of your dashboard here)

⭐ Future Enhancements

Automatic irrigation pump control

Weather-based crop prediction

Mobile app version

Multi-sensor support (RS485 daisy chaining)

👨‍💻 Developer

Karthick S
SRM Valliammai Engineering College
