# ⚡ PULSE — Global Emergency GIS Dispatch & AVL Tree Navigation System



<p align="center">

  <img src="https://raw.githubusercontent.com/25A31A05HH/PULSE/main/Screenshot%202026-11-01%20162410.jpg" alt="PULSE Emergency GIS Dispatcher Dashboard" width="100%" style="border-radius: 12px; border: 1px solid #334155;">

</p>



**PULSE** is a high-performance emergency medical dispatch web application and C++ algorithm core system. Designed for critical emergency response units, it integrates high-resolution geospatial satellite mapping (Esri Imagery), full patient address geocoding, self-balancing AVL Tree hospital indexing, Haversine distance telemetry, and real-time Web Speech API voice guidance.



---



## 🔗 Live Application & Repository



* 🌐 **Live Web Application:** [https://25a31a05hh.github.io/PULSE/](https://25a31a05hh.github.io/PULSE/)

* 📦 **GitHub Repository:** [`25A31A05HH/PULSE`](https://github.com/25A31A05HH/PULSE)



---



## 👨‍💻 Developer & Architect



* **Developed & Designed by:** **Surimalla Venkata Tejaswi**

* **Project Type:** Professional GIS & Data Structures Emergency Dispatch System



---



## 🚀 Core Features



### 1. 🛰️ Esri High-Resolution Satellite Map Engine

* **High-Res Satellite Tiles:** Defaults to **Esri World Imagery** with an official transportation and boundary label overlay.

* **Interactive Map Controls:** Allows operators to switch between Satellite, Dark Mode, and OpenStreetMap layers.

* **Click-to-Pin Location:** Relocate patient emergency calls directly by clicking anywhere on the map or dragging the marker.



### 2. 📍 Patient Address Input & Geocoding

* **Full Address / Landmark Search:** Patients or operators can enter street addresses, landmarks, or town names (e.g., *"Bhanugudi Junction, Kakinada"*).

* **Nominatim Engine Integration:** Geocodes address strings into exact Latitude/Longitude coordinates dynamically.

* **Manual Coordinate Overrides:** Supports direct numerical entry for GPS Latitude and Longitude.



### 3. 🌳 Self-Balancing AVL Tree Core

* **O(log N) Optimal Hospital Querying:** Guarantees logarithmic lookup times for nearest available hospital nodes.

* **Dynamic Rotation Metrics:** Displays live AVL Tree height, rotation events (LL, RR, LR, RL), and node capacity indicators on the telemetry dashboard.



### 4. 🚑 Telemetry & Real-Time Dispatch Routing

* **Haversine Distance Formula:** Computes spherical distance between patient coordinates and candidate hospitals.

* **Route Polyline Overlay:** Renders dashed navigation polylines showing the optimal path on the map.

* **Animated Ambulance Routing:** Simulates live dispatch vehicle movement from hospital to patient destination.

* **Web Speech API:** Provides hands-free audio announcements of dispatch decisions and arrival ETAs.



---



## 📊 System Architecture & Flowchart



```text

                       +-----------------------------------+

                       |    1. Operator / Emergency Call   |

                       |  (Address Search / GPS Input)     |

                       +-----------------+-----------------+

                                         |

                                         v

                       +-----------------------------------+

                       |  2. Geocoding / Nominatim Engine  |

                       |  (Converts Address -> Lat/Lng)    |

                       +-----------------+-----------------+

                                         |

                                         v

                       +-----------------------------------+

                       |  3. Esri Satellite Mapping Grid   |

                       |  (Leaflet Render & Marker Pin)    |

                       +-----------------+-----------------+

                                         |

                                         v

                       +-----------------------------------+

                       | 4. Self-Balancing AVL Tree Core   |

                       |   - Hospital Indexing O(log N)    |

                       |   - Dynamic Rotation Balance      |

                       +-----------------+-----------------+

                                         |

                                         v

                       +-----------------------------------+

                       | 5. Telemetry & Routing Engine     |

                       |   - Haversine Great-Circle Dist   |

                       |   - ETA Calculation & Path Lines  |

                       +-----------------+-----------------+

                                         |

                                         v

                       +-----------------------------------+

                       | 6. Optimal Dispatch & Navigation  |

                       |   - Vehicle Animation             |

                       |   - Web Speech API Voice Guidance |

                       +----------------+------------------+

```



---



## 📂 Repository File Structure



```text

PULSE/

├── index.html                             # Single-File Interactive GIS Web Application

├── pulse.cpp                              # C++ Backend Engine (AVL Tree & Algorithm Logic)

├── PULSE_Professional_15_Slide_Presentation.pptx # Executive 15-Slide Presentation Deck

├── README.md                              # System Documentation & Architecture Overview

└── Screenshot 2026-11-01 162410.jpg      # Dashboard Screenshot Image

```



---



## 🛠️ How to Apply to GitHub



1. Open your repository `https://github.com/25A31A05HH/PULSE`.

2. Ensure your uploaded image file name matches `Screenshot 2026-11-01 162410.jpg`.

3. Open `README.md`, click the edit (pencil) icon, paste this entire text, and click **Commit changes...**.



---



## 📜 License & Credits



Designed, architected, and built by **Surimalla Venkata Tejaswi**. Open for academic review, professional evaluation, and emergency technology portfolio demonstration.
