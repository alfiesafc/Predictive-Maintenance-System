# Predictive-Monitoring-System

A predictive monitoring and fault detection system utilizing an ESP32, physical telemetry hardware, and serial data acquisition for real-time sensor tracking.

---

## Project Overview

This project demonstrates a multi-sensor data acquisition and anomaly detection pipeline. The system tracks real-time operational metrics including temperature, vibration, and motor RPM to detect anomalies, log thermal or mechanical instabilities, and trigger visual warning alerts.

---

## Hardware & Rig Demonstration

> NOTE: *The video playback is set at 2x speed in order to comply with GitHub's upload limit.*

View the video files (`RPM.mp4`, `ACCELERATION.mp4`, and `TEMPERATURE.mp4`) in the repository for the respective sensor demonstrations.

---

## Features

* **Real-Time Sensor Monitoring:** Live temperature, vibration ($\text{m/s}^2$), and motor RPM tracking.
* **Fault Detection & Warnings:** Automatically flags abnormal behavior such as thermal instability, sudden RPM drops, or vibration faults.
* **OLED Display Interface:** Visualizes system status, normal operating metrics, and fault alerts directly on-device.
* **Manual & Serial Controls:** Integrated physical push buttons alongside a robust serial command pipeline (`RUN`) supporting fallback simulation modes.

---

## System Resilience & Fallback Mode

In the event of physical peripheral disruption, the firmware supports an integrated serial data collection via ESP32. This ensures continuous data acquisition, threshold monitoring, and visualization integrity without requiring a screen to be functional as demonstrated in the video walkthroughs.

---

## Written Report

* **Technical Write-up:** Detailed documentation of system architecture, validation, and graceful degradation strategies.
* **Hardware Analysis:** Documentation of the integration between the ESP32 microcontroller, sensors, and motor components.
* **Data Analysis:** Breaks down the findings of the telemetry system including threshold limits and fault triggers.

View `PMS.docx` for the complete detailed report validating the project.

---

## Scripts

* `esp32_firmware`: C++ firmware for the ESP32 handling data collection, sensor parsing, threshold logic, and serial telemetry output.
* `python_dashboard`: Data acquisition and visualization pipeline outlining live metrics and potential faults.
