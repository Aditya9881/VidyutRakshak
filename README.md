# ⚡ VidyutRakshak IoT
### IoT-Based Transmission Line Fault Detection System Using Arduino (for Rural Safety)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow?style=for-the-badge&logo=javascript)
![Arduino](https://img.shields.io/badge/Arduino-Uno-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-Realtime%20Database-orange?style=for-the-badge&logo=firebase)
![Vercel](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel)

**Department of Electrical Engineering**  
**Babu Banarasi Das Northern India Institute of Technology (BBDNIIT)**  
*(Affiliated to Dr. A.P.J. Abdul Kalam Technical University, Lucknow)*  

- **Under Guidance of:** Mr. Pradeep Kumar Verma (Assistant Professor)
- **Project Team:**
  - Ankit Yadav (Roll: 2300560200004)
  - Shivendra Singh (Roll: 2300560200032)

---

## 🌾 The Problem: Rural Line Safety is a Life Safety Issue
In rural areas, transmission and distribution lines often pass directly over open agricultural fields, village pathways, and irrigation canals. Undetected line breaks and fallen conductors pose grave risks:
1. **Farmers at Direct Risk**: Accidental contact during farming, plowing, or using tractors and metal ladders.
2. **Livestock Hazard**: Cattle wandering in open pastures electrocuted by high step-potential.
3. **Delayed Response**: Traditional faults are reported manually by villagers only after accidents occur.

---

## ⚡ Solution & Working Principle
**VidyutRakshak IoT** continuously monitors 3-phase line parameters:
- **Current Sensors (ACS712)**: Detect overcurrent and short circuits.
- **Voltage Sensors (PT / Dividers)**: Detect voltage drops and line breaks.
- **Conductor Temperature Sensor**: Detects conductor overheating and electrical fire risks.
- **Microcontroller (Arduino Uno)**: Analyzes real-time sensor data and compares with preset safety thresholds.
- **Protective Isolation**: Trips the 5V electromagnetic relay in **`< 4 seconds`** to isolate the hazardous section before injury occurs.
- **IoT & GSM Alerting**: Pushes real-time status to the cloud dashboard and dispatches emergency SMS alerts to the grid control room and village heads.

---

## ✨ Key Features
- **Farmer & Rural Safety Alert System**: Highlights hazard perimeters, fallen wire warnings, and farm machinery advisories.
- **Arduino Uno 16x2 LCD Digital Twin**: Visualizes real-time Arduino display and indicator LEDs (Normal, Fault, Relay Coil, Buzzer).
- **Rural Feeder Geographic Map**: Interactive SVG profile showing sub-stations, intermediate transmission poles (T1–T4), and exact fault distances.
- **Real-Time VI Dynamics Waveforms**: Live Chart.js telemetry showing instantaneous current surges and voltage sags.
- **Simulation Sandbox**: Interactive testbench to inject single line-to-ground (L-G), line-to-line (L-L), 3-phase, and fire events.
- **Tested Prototype Results**:
  - Trip Speed: **`< 4 seconds`**
  - Detection Accuracy: **`~98%`**
  - Fault Identification: **`3/3 (Overcurrent, L-G, L-L)`**

---

## 🚀 Deployment on Vercel

### Option 1: Automatic GitHub Import
1. Push this repository to GitHub.
2. Go to [Vercel](https://vercel.com) and click **"Add New Project"**.
3. Import your repository: `https://github.com/Aditya9881/VidyutRakshak.git`.
4. Keep the default settings (Framework Preset: **Other** / Root Directory: `./`).
5. Click **Deploy**. Your site will be live instantly with a free `.vercel.app` URL and global CDN!

### Option 2: Vercel CLI
```bash
npm i -g vercel
vercel
```

---

## 📜 License
Licensed under the **MIT License**.
