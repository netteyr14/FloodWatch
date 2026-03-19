# FloodWatch (Under Developemnt)

[![Python](https://img.shields.io/badge/Python-3.11.5-red?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![LightGBM](https://img.shields.io/badge/LightGBM-4.6.0-red?style=for-the-badge)](https://lightgbm.readthedocs.io/)
[![Waitress](https://img.shields.io/badge/Waitress-3.0.2-red?style=for-the-badge)](https://docs.pylonsproject.org/projects/waitress/en/stable/)
[![Flutter](https://img.shields.io/badge/Flutter-3.35.7-orange?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev/)
[![Docker](https://img.shields.io/badge/Docker-29.2.0-blue?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![NGINX](https://img.shields.io/badge/NGINX-1.28.0-blue?style=for-the-badge&logo=nginx&logoColor=white)](https://nginx.org/)
[![Cloudflared](https://img.shields.io/badge/Cloudflared-2025.8.1-blue?style=for-the-badge)](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0.35-yellowgreen?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)

**Research Paper Reference:**  
*"Real-Time Flood Monitoring System with Water Level Forecasting using LoRaWAN-Based Wireless Sensor Network"*

---

## Overview
FloodWatch is an IoT-based flood monitoring system that detects rising water levels in real-time, generates forecasts, and sends alerts to residents and barangay officials. It integrates distributed sensor nodes, wireless LoRaWAN communication, a containerized cloud backend, and Flutter applications for community users and administrators.

## System Screenshots

<p align="center">
  <img src="assets/github_ss1.png" width="700"/>
</p>

<p align="center">
  <img src="assets/github_ss7.png" width="700"/>
</p>

<p align="center">
  <img src="assets/github_ss2.png" width="300"/>
  <img src="assets/github_ss3.png" width="300"/>
</p>

<p align="center">
  <img src="assets/github_ss4.png" width="269" height="268" style="margin-right: 10px;" />
  <img src="assets/github_ss5.png" width="269" height="200" style="margin-right: 10px;" />
  <img src="assets/github_ss6.png" width="269" height="200" />
</p>

---

## System Components

- **Resident Application** – A cross-platform interface built with Flutter for web and mobile devices, allowing community members to view real-time flood data, forecasts, and receive alerts.
- **Admin Dashboard** – A desktop-based application developed using Flutter, designed for monitoring system status, managing data, and supporting decision-making for authorities.
- **Backend API** – A containerized server powered by Docker and Python, utilizing Waitress and NGINX for request handling, MySQL for data storage, and LightGBM for flood prediction and forecasting.
- **Sensor Nodes (LoRa32)** – Distributed field units installed on monitoring towers, equipped with FMCW radar, rain sensors, and anemometers. These nodes operate on a 12V 9Ah power system with solar support and communicate via LoRa-based wireless transmission.

---

## System Architecture

```text
Tower Sensors (LoRa32) → LoRa32 Gateway → Backend API (Docker) → MySQL Database → Applications (Resident Web/App / Admin Dashboard)
```

---

## Repositories (Private)

The backend, mobile, and desktop applications are maintained in private repositories due to security and research considerations.

Access can be requested via:
753951852456arvin@gmail.com

---
