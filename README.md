# FloodWatch (Under Developemnt)

### Core Technologies
[![Python](https://img.shields.io/badge/Python-3.11.5-red?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Flutter](https://img.shields.io/badge/Flutter-3.35.7-orange?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev/)
[![LightGBM](https://img.shields.io/badge/LightGBM-4.6.0-red?style=for-the-badge)](https://lightgbm.readthedocs.io/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0.35-yellowgreen?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)

### Infrastructure & Deployment
[![Docker](https://img.shields.io/badge/Docker-29.2.0-blue?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![NGINX](https://img.shields.io/badge/NGINX-1.28.0-blue?style=for-the-badge&logo=nginx&logoColor=white)](https://nginx.org/)
[![Waitress](https://img.shields.io/badge/Waitress-3.0.2-red?style=for-the-badge)](https://docs.pylonsproject.org/projects/waitress/en/stable/)
[![Cloudflared](https://img.shields.io/badge/Cloudflared-2025.8.1-blue?style=for-the-badge)](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/)

**Research Paper Reference:**  
*"Real-Time Flood Monitoring System with Water Level Forecasting using LoRaWAN-Based Wireless Sensor Network"*

---

## Overview
FloodWatch is an IoT-based flood monitoring system that detects rising water levels in real-time, generates forecasts, and sends alerts to residents and barangay officials. 

Unlike traditional flood monitoring systems, FloodWatch integrates machine learning-based forecasting and low-power LoRaWAN communication to enable predictive, real-time community alerts even in low-connectivity areas. It combines distributed sensor nodes, wireless communication, a containerized cloud backend, and Flutter applications for both residents and administrators.

## System Screenshots

## System Screenshots

<p align="center"><b>Resident Mobile Interface</b></p>
<p align="center">
  <img src="assets/github_ss1.png" width="700"/>
</p>

<p align="center"><b>Admin Dashboard</b></p>
<p align="center">
  <img src="assets/github_ss7_new.png" width="700"/>
</p>

<p align="center"><b>Mobile App: Node & Data Views</b></p>
<p align="center">
  <img src="assets/github_ss2.png" width="300"/>
  <img src="assets/github_ss3.png" width="300"/>
</p>

<p align="center"><b>Dashboard: Sensor & Forecast Views</b></p>
<p align="center">
  <img src="assets/github_ss4.png" width="269" height="268" style="margin-right: 10px;" />
  <img src="assets/github_ss5.png" width="269" height="200" style="margin-right: 10px;" />
  <img src="assets/github_ss6.png" width="269" height="200" />
</p>

---

## System Components

- **Resident Application** – Cross-platform Flutter app for web and mobile. Allows residents to view real-time flood data, forecasts, and alerts.
- **Admin Dashboard** – Desktop Flutter app for monitoring system status, managing sensor data, and supporting decision-making for authorities.
- **Backend API** – Containerized Python server using Docker, Waitress, and NGINX. Handles data processing, storage (MySQL), and flood prediction via LightGBM.
- **Sensor Nodes (LoRa32)** – Field units with FMCW radar, rain sensors, and anemometers. Powered by 12V 9Ah with solar support, sending data via LoRaWAN.

---

## System Architecture

```text
Sensor Nodes (LoRa32)
        ↓
LoRa Gateway
        ↓
Backend API (Docker + Python)
        ↓
Data Processing & LightGBM Forecasting
        ↓
MySQL Database
        ↓
REST/WebSocket API
        ↓
Resident App / Admin Dashboard
```

---

## Features
- Real-time water level monitoring
- Flood prediction using LightGBM
- Mobile & web-based alerts
- Offline-capable LoRa communication
- Admin monitoring dashboard with analytics

---

## Repositories (Private)

The backend, mobile, and desktop applications are maintained in private repositories due to security and research considerations.

Access can be requested via:
753951852456arvin@gmail.com

---
