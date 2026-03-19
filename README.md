# FloodWatch

**Research Paper Reference:**  
*"Real-Time Flood Monitoring System with Water Level Forecasting using LoRaWAN-Based Wireless Sensor Network"*

---

## Overview
FloodWatch is an IoT-based flood monitoring system designed to detect rising water levels in real-time, provide forecasts, and alert both residents and barangay officials. The system integrates sensor nodes, wireless communication, a cloud backend, and intuitive applications for both community users and administrative officers.

---

## System Components
- **📱 Resident Application** – Flutter Web & Mobile for community users  
- **🖥️ Admin Dashboard** – Flutter Desktop for barangay officers  
- **⚙️ Backend API** – Containerized (Docker) backend with database and alert services  
- **📡 Sensor Nodes** – Microcontroller-based with LoRaWAN/GSM for data collection

---

## System Architecture

```text
Sensor Nodes → Backend API (Docker) → Database → Applications (Resident App / Admin Dashboard)
