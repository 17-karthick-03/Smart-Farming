IOT_AI_ENABLED_PRECISION_FARMING_SYSTEM

The purpose of this project is to build a smart precision farming system using a Raspberry Pi 5, a 6-in-1 RS485 Soil Sensor, and AI (Gemini) to provide real-time soil monitoring, intelligent crop recommendations, and automated nutrient alerts.

REQUIREMENTS

⭐ Raspberry Pi 5
⭐ RS485 Soil Sensor (6-in-1: Moisture, Temperature, pH, Nitrogen, Phosphorus, Potassium)
⭐ USB to RS485 Converter (to connect the sensor to Raspberry Pi)
⭐ 5V 3A Power Adapter for Raspberry Pi
⭐ 12V Power Supply for Soil Sensor
⭐ Jumper wires for connections
⭐ Wi-Fi network (for API + dashboard + email alerts)

SETUP INSTRUCTIONS
1. Clone the Project

Upload all files (including app.py, templates, static files) to your Raspberry Pi 5.

2. Install Required Libraries
pip install Flask minimalmodbus python-dotenv google-generativeai weasyprint

3. Connect the Components

RS485 Soil Sensor:
Connect the sensor using the USB → RS485 converter to the Raspberry Pi.

Power:

Raspberry Pi → 5V adapter

Soil Sensor → 12V adapter

4. Configure the Environment

Create a .env file and add:

GEMINI_API_KEY=your_key_here
EMAIL_SENDER=your_email
EMAIL_PASSWORD=your_app_password
SMTP_SERVER=smtp.gmail.com
SMTP_PORT=587

5. Run the Application
python3 app.py


Open the dashboard in your browser:

http://<raspberry-pi-ip>:5001

HOW IT WORKS
🌱 Real-Time Sensor Reading

Reads moisture, temperature, pH, and NPK levels every 30 seconds via Modbus.

🧠 AI Soil Analysis

Gemini AI analyzes your soil values and recommends suitable crops.

🔍 Crop Suitability Check

User can enter any crop name to see if the soil matches its ideal conditions.

📄 PDF Reports

Soil Sensor Report

AI Recommendation Report

User Crop Analysis Report

All are auto-generated using WeasyPrint.

🔔 Continuous Monitoring

You can select a crop to monitor.
If soil nutrients move outside the ideal range, the system sends email alerts (once every 24 hrs).

💬 Smart Gardening Chatbot

Assists users with terrace farming questions.

FINAL NOTES

This system provides an end-to-end smart farming experience by combining IoT, AI, real-time soil data, and automation.
Useful for home gardening, terrace farming, hydroponics, and precision agriculture. 🌾💡
