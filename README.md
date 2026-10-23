# FloodWatch

### Core Technologies
[![Python](https://img.shields.io/badge/Python-3.11.5-red?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![LightGBM](https://img.shields.io/badge/LightGBM-4.6.0-red?style=for-the-badge)](https://lightgbm.readthedocs.io/)
[![Flutter](https://img.shields.io/badge/Flutter-3.35.7-orange?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev/)
[![C++](https://img.shields.io/badge/C++-20-blue?style=for-the-badge&logo=c%2B%2B&logoColor=white)](https://isocpp.org/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0.35-yellowgreen?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)

### Infrastructure & Deployment
[![Gunicorn](https://img.shields.io/badge/Gunicorn-25.3.0-red?style=for-the-badge&logo=gunicorn&logoColor=white)](https://gunicorn.org/)
[![Docker](https://img.shields.io/badge/Docker-29.2.0-blue?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![NGINX](https://img.shields.io/badge/NGINX-1.28.0-blue?style=for-the-badge&logo=nginx&logoColor=white)](https://nginx.org/)
[![Cloudflared](https://img.shields.io/badge/Cloudflared-2025.8.1-blue?style=for-the-badge&logo=cloudflare&logoColor=white)](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/)

**Research Paper Reference:**  
*"Real-Time Flood Monitoring System with Water Level Forecasting using LoRa-based Wireless Sensor Network" (in progress)*

---

## Overview
FloodWatch is an IoT-based flood monitoring system that tracks rising water levels in real time, forecasts flood risk, and sends timely alerts to residents and barangay officials.

Unlike conventional monitoring setups, it pairs machine learning forecasting with low-power LoRa P2P communication, delivering both predictive and real-time community alerts. The system combines distributed sensor nodes/towers, wireless networking, a containerized backend, and Flutter apps for residents and administrators.

## System Screenshots

<p align="center"><b>Frontend: Admin Dashboard</b></p>
<p align="center">
  <img src="updated_ui/desktop_app/desktop_login.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_expanded_close.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_expanded_open.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_details_close.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_details_open.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_operations_close.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_operations_open.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_alerts.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_profile.jpg" width="700"/>
  <img src="updated_ui/desktop_app/desktop_about_us.jpg" width="700"/>
</p>

<p align="center"><b>Admin Reports: XLSX Output</b></p>
<p align="center">
  <img src="assets/xlsx_reports.png" width="700"/>
  <img src="assets/xlsx_reports-1.png" width="700"/>
</p>

<p align="center"><b>Backend: "floodwatch-backend" Container</b></p>
<p align="center">
  <img src="updated_ui/ssh_backend/backend.png" width="700"/>
</p>

<p align="center"><b>Frontend: Mobile App / Web App</b></p>
<p align="center">
  <img src="updated_ui/mobile_app/mobile_home_1.jpg" width="300"/>
  <img src="updated_ui/mobile_app/mobile_home_2.jpg" width="300"/>
  <img src="updated_ui/mobile_app/mobile_home_3.jpg" width="300"/>
  <img src="updated_ui/mobile_app/mobile_alerts.jpg" width="300"/>
  <img src="updated_ui/mobile_app/mobile_profile.jpg" width="300"/>
  <img src="updated_ui/mobile_app/mobile_about_us.jpg" width="300"/>
</p>
<hr>
<p align="center">
  <img src="updated_ui/desktop_web/desktop_web_home.jpg" width="700"/>
  <img src="updated_ui/desktop_web/desktop_web_alerts.jpg" width="700"/>
  <img src="updated_ui/desktop_web/desktop_web_profile.jpg" width="700"/>
  <img src="updated_ui/desktop_web/desktop_web_about_us.jpg" width="700"/>
</p>

<p align="center">
  <strong>Try the FloodWatch Web App</strong><br/>
  <a href="https://floodwatchph.me">https://floodwatchph.me</a>
</p>

<p align="center"><b>3D-Model: Front, Side, Top</b></p>
<p align="center">
  <img src="assets/model_front.png" width="269" height="200" style="margin-right: 10px;" />
  <img src="assets/model_side.png" width="269" height="200" style="margin-right: 10px;" />
  <img src="assets/model_top.png" width="269" height="200" />
</p>

---

## System Components

- **Resident Application** – Cross-platform Flutter app for web and mobile. Allows residents to view real-time flood data, forecasts, and alerts.
- **Admin Dashboard** – Desktop Flutter app for monitoring system status, managing sensor data, and supporting decision-making for authorities.
- **Backend API** – Containerized Python server using Docker, Gunicorn, and NGINX. Handles data processing, storage (MySQL), and flood prediction via LightGBM.
- **Sensor Nodes (LoRa32)** – Field units with FMCW radar, rain sensors, and anemometers. Powered by 12V 9Ah VRLA lead-acid battery with solar support, sending data via LoRa P2P.

---

## System Architecture

```text
Sensor Nodes (LoRa32 TX)
        ↓ LoRa P2P
Base Receiver (LoRa32 RX)
        ↓
_____________________________________________________________
Backend API (Docker + NGINX + Python + Cloudflare tunneling)
        ↓
MySQL Database
        ↓
Data Processing & LightGBM Forecasting
        ↓
_____________________________________________________________
REST/WebSocket API
        ↓
Resident App / Admin Dashboard
```

---

## Features
- Real-time water level monitoring
- Flood prediction using LightGBM
- Mobile & web-based alerts
- Offline-capable operation over LoRa and the local network (Desktop Admin App)
- Admin monitoring dashboard with analytics

---

## Repositories (Private)

The backend, mobile, and desktop applications are maintained in private repositories due to security and research considerations.

Access can be requested via email:
753951852456arvin@gmail.com

---
