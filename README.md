# mapping-and-localization-matlab
2D Mapping and Robot Localization using MATLAB Robotics Toolbox with LiDAR and Particle Filter
# 🗺️ Mapping and Localization using MATLAB (Robotics)

This project demonstrates **2D Mapping and Robot Localization** using MATLAB Robotics System Toolbox.
It builds an **occupancy grid map** from LiDAR data and estimates the robot’s pose using **particle filter based localization**.

---

## 📌 Project Overview

**Mapping and Localization** refers to:

* Building a map of an environment using sensor data (LiDAR)
* Estimating the robot’s position inside that map

This project uses:

* Occupancy Grid Mapping
* Particle Filter Localization
* 2D LiDAR Scan Data

---

## 🧠 Core Concepts

### 🗺️ Mapping

* Uses `binaryOccupancyMap`
* Inserts LiDAR rays into the map using `insertRay`
* Each cell represents free or occupied space

### 📍 Localization

* Uses `stateEstimatorPF` (Particle Filter)
* Robot pose is estimated using `predict` and `correct` steps

---

## 🧩 Workflow

1. Generate or load LiDAR data
2. Build occupancy grid map
3. Initialize particle filter
4. Estimate robot pose over time
5. Plot map and robot trajectory

---

## 📁 Project Structure

```
mapping-and-localization-matlab/
├── main.m
├── build_map.m
├── localize_robot.m
├── generate_fake_lidar.m
├── data/
│   └── lidar_scans.mat
└── results/
    ├── map.png
    └── localization.png
```

---

## ▶️ How to Run

1. Open MATLAB
2. Open this project folder
3. Run:

```matlab
main
```

---

## 🧰 Tools & Functions Used

* `binaryOccupancyMap`
* `lidarScan`
* `insertRay`
* `stateEstimatorPF`
* `predict`, `correct`

---

## 📚 Reference

Based on MathWorks documentation:
Mapping and Localization — MATLAB Robotics System Toolbox

**Tanshya Mishra**
Computer Science Graduate, VIT Vellore
Interested in AI, ML, Robotics, and Intelligent Systems
