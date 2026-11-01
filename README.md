# ⚡ PULSE — Global Emergency GIS Dispatch & AVL Tree Navigation System

<p align="center">
  <img src="https://raw.githubusercontent.com/25A31A05HH/PULSE/main/pulse-dashboard.jpg" alt="PULSE Emergency GIS Dispatcher Dashboard" width="100%">
</p>

<p align="center">
  <strong>Intelligent Emergency Dispatch • Geospatial Intelligence • Advanced Data Structures</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Project-PULSE-00BFFF?style=for-the-badge">
  <img src="https://img.shields.io/badge/Language-C++-00599C?style=for-the-badge&logo=cplusplus">
  <img src="https://img.shields.io/badge/Frontend-HTML5-orange?style=for-the-badge&logo=html5">
  <img src="https://img.shields.io/badge/Mapping-Leaflet-199900?style=for-the-badge&logo=leaflet">
  <img src="https://img.shields.io/badge/Status-Academic%20Prototype-success?style=for-the-badge">
</p>

---

## 🌐 Project Overview

**PULSE (Global Emergency GIS Dispatch & AVL Tree Navigation System)** is an interactive emergency medical dispatch application designed to demonstrate how geospatial technologies, data structures, and intelligent routing algorithms can support emergency response coordination.

The system integrates interactive GIS mapping, patient location geocoding, self-balancing AVL Tree hospital indexing, Haversine distance calculations, ambulance route visualization, and browser-based voice guidance.

PULSE demonstrates the combination of a web-based GIS interface and a C++ algorithm core to explore efficient hospital selection and emergency dispatch workflows.

## 🔗 Live Application & Repository

- 🌐 **Live Web Application:** [Launch PULSE](https://25a31a05hh.github.io/PULSE/)
- 📦 **GitHub Repository:** [25A31A05HH/PULSE](https://github.com/25A31A05HH/PULSE)

---

## 👨‍💻 Developer & Architect

| Detail | Information |
|---|---|
| Developer | **Surimalla Venkata Tejaswi** |
| Project Name | PULSE |
| Project Domain | GIS, Emergency Dispatch & Data Structures |
| Core Algorithm | AVL Tree |
| Backend Algorithm Implementation | C++ |
| Frontend | HTML, CSS & JavaScript |
| Deployment | GitHub Pages |

**Project Objective:** To demonstrate how efficient data structures and geospatial technologies can be combined to support emergency location analysis and hospital dispatch decision-making.

---

## 🚀 Core Features

### 1. 🛰️ Esri High-Resolution Satellite Mapping

- Uses Esri World Imagery for satellite-based geographical visualization.
- Supports multiple map layers, including Satellite, Dark Mode, and OpenStreetMap.
- Provides interactive zooming, panning, and map navigation.
- Allows operators to identify emergency locations visually.
- Supports click-to-pin patient location selection.
- Enables marker repositioning through interactive map controls.

### 2. 📍 Patient Address Input & Geocoding

- Supports street addresses, landmarks, and location names.
- Integrates the Nominatim geocoding service to convert address descriptions into geographical coordinates.
- Supports manual latitude and longitude entry.
- Enables emergency location selection through map interaction.
- Displays patient coordinates for geographical analysis.

**Example Location:** Bhanugudi Junction, Kakinada.

### 3. 🌳 Self-Balancing AVL Tree Core

PULSE demonstrates AVL Tree-based hospital indexing for efficient data organization and searching.

**Key capabilities:**

- Self-balancing Binary Search Tree implementation.
- Efficient insertion and searching operations.
- Dynamic height calculation.
- Balance factor monitoring.
- Four AVL Tree rotations:
  - LL – Left Left Rotation
  - RR – Right Right Rotation
  - LR – Left Right Rotation
  - RL – Right Left Rotation
- Tree height and balancing metrics.

**Time Complexity:**

| Operation | Average/Worst-case Complexity |
|---|---|
| Search | O(log N) |
| Insertion | O(log N) |
| Deletion | O(log N) |
| Tree Traversal | O(N) |

AVL Trees maintain logarithmic height, making them suitable for efficient indexed data retrieval.

### 4. 🚑 Emergency Dispatch & Routing Engine

- Calculates geographical distances between patient locations and candidate hospitals.
- Uses the Haversine formula for great-circle distance estimation.
- Identifies candidate hospitals based on calculated proximity.
- Visualizes dispatch routes using map polylines.
- Simulates ambulance movement between locations.
- Displays dispatch telemetry and estimated travel information.

**Important:** Geographical distance is not the same as actual road distance. The prototype's distance-based selection should not be interpreted as a verified fastest-road-route recommendation.

### 5. 🔊 Real-Time Voice Guidance

PULSE incorporates the browser Web Speech API to demonstrate voice-based dispatch announcements.

- Text-to-speech announcements.
- Dispatch decision notifications.
- Hands-free audio guidance.
- Browser-supported voice output.

### 6. 📊 Live Telemetry Dashboard

The dashboard demonstrates important system metrics, including:

- Patient geographical coordinates.
- Hospital indexing information.
- AVL Tree height.
- Rotation event metrics.
- Distance calculations.
- Dispatch information.
- Navigation and routing visualization.

---

## 🏗️ System Architecture & Workflow

The PULSE system follows a structured emergency dispatch workflow.

```text
              ┌───────────────────────────────────┐
              │  1. Emergency Call / Operator     │
              │     Address Search / GPS Input    │
              └─────────────────┬─────────────────┘
                                │
                                ▼
              ┌───────────────────────────────────┐
              │  2. Geocoding Engine               │
              │     Nominatim Address Conversion  │
              │     Latitude / Longitude          │
              └─────────────────┬─────────────────┘
                                │
                                ▼
              ┌───────────────────────────────────┐
              │  3. GIS Mapping Engine             │
              │     Leaflet + Esri Satellite       │
              │     Patient Location Visualization│
              └─────────────────┬─────────────────┘
                                │
                                ▼
              ┌───────────────────────────────────┐
              │  4. AVL Tree Hospital Indexing     │
              │     Hospital Data Organization    │
              │     Self-Balancing Operations     │
              └─────────────────┬─────────────────┘
                                │
                                ▼
              ┌───────────────────────────────────┐
              │  5. Distance & Routing Engine      │
              │     Haversine Distance Calculation│
              │     Dispatch Route Visualization  │
              └─────────────────┬─────────────────┘
                                │
                                ▼
              ┌───────────────────────────────────┐
              │  6. Emergency Dispatch Interface   │
              │     Ambulance Movement Simulation │
              │     Voice Guidance & Telemetry    │
              └───────────────────────────────────┘
```

---

## 🧮 Key Algorithms

### A. AVL Tree Algorithm

The AVL Tree is a self-balancing Binary Search Tree in which the height difference between the left and right subtrees of every node is at most one.

**Balance Factor:**

```cpp
Balance Factor = Height(Left Subtree) - Height(Right Subtree)
```

A node is balanced when its balance factor is -1, 0, or +1.

### B. Haversine Distance Formula

The Haversine formula calculates the great-circle distance between two geographical coordinates.

\[
a = \sin^2\left(\frac{\Delta\phi}{2}\right)
+\cos(\phi_1)\cos(\phi_2)
\sin^2\left(\frac{\Delta\lambda}{2}\right)
\]

\[
d = 2R\arctan2(\sqrt{a},\sqrt{1-a})
\]

Where:

- \(R\) = Earth's mean radius.
- \(\phi_1,\phi_2\) = Latitudes in radians.
- \(\lambda_1,\lambda_2\) = Longitudes in radians.
- \(d\) = Great-circle distance.

### C. Geocoding

The Nominatim service converts human-readable location descriptions into geographical latitude and longitude coordinates.

---

## 🛠️ Technologies & Tools Used

| Technology | Purpose |
|---|---|
| C++ | AVL Tree and algorithm implementation |
| HTML5 | Web application structure |
| CSS3 | Dashboard styling and responsive interface |
| JavaScript | Application logic and interactions |
| Leaflet.js | Interactive GIS mapping |
| Esri World Imagery | Satellite map visualization |
| OpenStreetMap | Open geographical map data |
| Nominatim | Address geocoding |
| Haversine Formula | Geographical distance calculation |
| Web Speech API | Voice announcements |
| GitHub | Source code management |
| GitHub Pages | Web application deployment |

---

## 📁 Project Directory Structure

```text
PULSE/
│
├── index.html
│   └── Single-File Interactive GIS Web Application
│
├── pulse.cpp
│   └── C++ Backend Engine (AVL Tree & Algorithm Logic)
│
├── PULSE_Professional_15_Slide_Presentation.pptx
│   └── Professional 15-Slide Project Presentation
│
├── README.md
│   └── Project Documentation & System Architecture
│
└── Screenshot 2026-11-01 162410.jpg
    └── Emergency Dispatch Dashboard Screenshot
```

---

## ⚙️ Running the Project

### 1. Run the Web Application

You can access the deployed application directly:

[Launch PULSE Web Application](https://25a31a05hh.github.io/PULSE/)

Alternatively, clone the repository:

```bash
git clone https://github.com/25A31A05HH/PULSE.git
```

Navigate into the project directory:

```bash
cd PULSE
```

Open `index.html` in your browser or use a local development server.

### 2. Compile and Run the C++ Core

Ensure that a C++ compiler such as GCC or MinGW is installed.

Compile:

```bash
g++ pulse.cpp -o pulse
```

Run on Windows:

```bash
pulse.exe
```

Run on Linux/macOS:

```bash
./pulse
```

---

## 🎯 Applications & Use Cases

PULSE demonstrates concepts relevant to:

- Emergency medical dispatch systems.
- Hospital location indexing.
- Geospatial information systems.
- Location-based service applications.
- Ambulance dispatch coordination.
- Algorithmic optimization.
- Real-time geographical visualization.
- Data Structures and Algorithms education.

---

## 🔮 Future Enhancements

Potential future improvements include:

- Integration with verified hospital databases.
- Real-time hospital bed and emergency department availability.
- Live GPS tracking through connected ambulance devices.
- Road-network-based shortest-path routing.
- Traffic-aware ambulance route optimization.
- Backend API integration.
- Secure patient information management.
- Multi-user emergency operator dashboard.
- Integration with verified emergency response services.

---

## ⚠️ Disclaimer

PULSE is an **academic prototype and portfolio demonstration**, developed to explore the integration of GIS mapping, AVL Trees, geographical distance calculations, and emergency dispatch concepts.

It is not a certified emergency medical dispatch platform and has not been validated for real-world emergency operations.

Hospital availability, ambulance locations, road travel times, and medical response decisions must be verified through authorized services before any operational use.

---

## 📜 License & Credits

**Designed, Architected, and Developed by Surimalla Venkata Tejaswi.**

PULSE is an independently developed academic and portfolio project.

### Third-Party Technologies & Acknowledgements

- [Esri](https://www.esri.com/) – Satellite imagery and mapping services.
- [Leaflet](https://leafletjs.com/) – Interactive mapping framework.
- [OpenStreetMap](https://www.openstreetmap.org/) – Open geographical map data.
- [Nominatim](https://nominatim.org/) – Geocoding services.
- Web Speech API – Browser-based speech synthesis.

Third-party technologies and geographical data remain subject to their respective licenses, attribution requirements, and usage policies.

### Project Information

| Category | Details |
|---|---|
| Project | PULSE |
| Developer | Surimalla Venkata Tejaswi |
| Year | 2026 |
| Domain | GIS & Emergency Dispatch |
| Implementation | C++ & Web Technologies |
| Project Status | Academic Prototype / Portfolio Demonstration |

---

<p align="center">
  <strong>⚡ PULSE — Connecting Location Intelligence with Emergency Response.</strong>
</p>

<p align="center">
  Developed with dedication by <strong>Surimalla Venkata Tejaswi</strong>
</p>

<p align="center">
  ⭐ If you find this project interesting, consider starring the repository!
</p>
