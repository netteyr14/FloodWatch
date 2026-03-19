# FloodWatch (Under Developemnt)

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge)
![Flutter](https://img.shields.io/badge/Flutter-3.13-blue?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-20.10-blue?style=for-the-badge)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?style=for-the-badge)

**Research Paper Reference:**  
*"Real-Time Flood Monitoring System with Water Level Forecasting using LoRaWAN-Based Wireless Sensor Network"*

---

## Overview
FloodWatch is an IoT-based flood monitoring system that detects rising water levels in real-time, generates forecasts, and sends alerts to residents and barangay officials. It integrates distributed sensor nodes, wireless LoRaWAN communication, a containerized cloud backend, and Flutter applications for community users and administrators.

## System Screenshots

<p float="left">
  <img src="assets/github_ss2.png" width="300" />
  <img src="assets/github_ss3.png" width="300" />
</p>

![Admin Dashboard](assets/github_ss1.png)


<p float="left">
  <img src="assets/github_ss4.png" width="280" height="280" />
  <img src="assets/github_ss5.png" width="350" height="210" />
  <img src="assets/github_ss6.png" width="350" height="210" />
</p>
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
