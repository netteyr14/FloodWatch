# FloodWatch

**Research Paper Reference:**  
*"Real-Time Flood Monitoring System with Water Level Forecasting using LoRaWAN-Based Wireless Sensor Network"*

---

## Overview
FloodWatch is an IoT-based flood monitoring system designed to detect rising water levels in real-time, generate forecasts, and provide alerts to both residents and barangay officials. The system integrates distributed sensor nodes, wireless communication via LoRaWAN, a containerized cloud backend, and intuitive applications for community users and administrative officers.

---

## System Components

- **📱 Resident Application** – Flutter Web & Mobile for residents  
- **🖥️ Admin Dashboard** – Flutter Desktop for barangay officers  
- **⚙️ Backend API** – Dockerized Python backend with database, prediction service, and alert handling  
- **📡 Sensor Nodes (LoRa32)** – Towers equipped with FMCW Radar, Rain Sensor (Tipping Bucket), and Anemometer, powered by a 12V 9Ah UPS battery with PWM charge controller

---

## System Architecture

```text
Tower Sensors (LoRa32) → LoRa32 Gateway → Backend API (Docker) → MySQL Database → Applications (Resident Web/App / Admin Desktop)
