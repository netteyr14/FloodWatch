# FloodWatch (Under Developemnt)

![Python](https://img.shields.io/badge/Python-3.11.5-blue?style=for-the-badge)
![Flutter](https://img.shields.io/badge/Flutter-3.35.7-blue?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-29.2-blue?style=for-the-badge)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?style=for-the-badge)

**Research Paper Reference:**  
*"Real-Time Flood Monitoring System with Water Level Forecasting using LoRaWAN-Based Wireless Sensor Network"*

---

## Overview
FloodWatch is an IoT-based flood monitoring system that detects rising water levels in real-time, generates forecasts, and sends alerts to residents and barangay officials. It integrates distributed sensor nodes, wireless LoRaWAN communication, a containerized cloud backend, and Flutter applications for community users and administrators.

## System Screenshots

<div style="text-align: center; margin-bottom: 20px;">
  <img src="assets/github_ss2.png" width="300" style="display: inline-block; margin-right: 10px;" />
  <img src="assets/github_ss3.png" width="300" style="display: inline-block;" />
</div>

![Admin Dashboard](assets/github_ss1.png)

<div style="text-align: center;">
  <img src="assets/github_ss4.png" width="280" height="280" style="margin-right: 10px;" />
  <img src="assets/github_ss5.png" width="355" height="210" style="margin-right: 10px;" />
  <img src="assets/github_ss6.png" width="355" height="210" />
</div>

---

## System Components

- **Resident Application** – Flutter Web & Mobile  
- **Admin Dashboard** – Flutter Desktop  
- **Backend API** – Dockerized Python backend with Waitress, MySQL, and LightGBM for prediction  
- **Sensor Nodes (LoRa32)** – Towers with FMCW Radar, Rain Sensor, and Anemometer powered by 12V 9Ah UPS

---

## System Architecture

```text
Tower Sensors (LoRa32) → LoRa32 Gateway → Backend API (Docker) → MySQL Database → Applications (Resident Web/App / Admin Dashboard)
```

## Repositories (Private)

- [FloodWatch Backend](https://github.com/netteyr14/CAPSTONE-FloodWatch-LightGBM)
- [FloodWatch Mobile App/Web_App](https://github.com/netteyr14/FloodWatch-Mobile-App)
- [FloodWatch_Desktop_App](https://github.com/netteyr14/FloodWatch-Desktop-App)

- [Request Access](mailto:753951852456arvin@gmail.com) on this email.
