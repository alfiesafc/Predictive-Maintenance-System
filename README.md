# Predictive-Monitoring-System

A predictive monitoring and fault detection system utilizing an ESP32, physical telemetry hardware, and serial data acquisition for real-time sensor tracking.

---

## Project Overview

This project demonstrates a multi-sensor data acquisition and anomaly detection pipeline. The system tracks real-time operational metrics including temperature, vibration, and motor RPM to detect anomalies, log thermal or mechanical instabilities, and trigger visual warning alerts[cite: 6, 7, 8].

---

## Hardware & Rig Demonstration

> NOTE: *The video playback is set to speed up to be ample to be uploaded within github's 25mb file limit*[cite: 9]

View this demonstration under the video files section of this repository[cite: 6, 7, 8].

---

## Features

* **Real-Time Sensor Monitoring:** Live temperature, vibration ($m/s^2$), and motor RPM tracking[cite: 6, 7, 8].
* **Fault Detection & Warnings:** Automatically flags abnormal behavior such as thermal instability, sudden RPM drops, or vibration faults[cite: 6, 7, 8].
* **OLED Display Interface:** Visualizes system status, normal operating metrics, and fault alerts directly on-device[cite: 8].
* **Manual Controls:** Integrated physical `MODE` and `RESET` push buttons for system control and recovery[cite: 4, 8].

---

## Written Report

* **Technical Write-up:** Detailed documentation of system architecture and validation.
* **Hardware Analysis:** Documentation of the integration between the ESP32 microcontroller, sensors, and motor components[cite: 6, 7, 8].
* **Data Analysis:** Breaks down the findings of the telemetry system including threshold limits and fault triggers.
* **Visualisation:** Thorough view through graphical representation, the physical rig structure, and the circuitry feeding the project[cite: 1, 2, 3, 4].

View documentation files within this repository.

---

## Scripts

* `project_A.ino` - ESP32 C++ firmware consisting of handling data collection, sensor parsing, and serial output[cite: 6, 7].
