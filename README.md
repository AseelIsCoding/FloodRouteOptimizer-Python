# 🌊 Flood-Aware Routing Optimization for Jeddah’s Rainy Days

## 📌 Overview
Jeddah, Saudi Arabia, frequently experiences severe **flash floods**, causing disruptions to transportation and endangering residents. This project presents a **flood-aware routing optimization model** to **enhance urban resilience** and ensure **safe transportation routes** during floods.

We explore **two optimization methods**:
- **✅ Exact Optimization (Linear Programming):** Guarantees optimal routes, ideal for **small-scale evacuations**.
- **⚡ Simulated Annealing:** Provides near-optimal solutions with faster computation, **scalable for large networks**.

## 🛠️ Methodology
The optimization problem is formulated to **maximize route safety** based on:
- **🛣️ Road Quality (q)** – Better roads are safer.
- **🚰 Drainage Efficiency (e)** – Roads with effective drainage are prioritized.
- **🌊 Flood Depth (d)** – Lower flood depth means safer travel.

Each road segment is **evaluated** using a **safety score**, and constraints ensure:
- **✅ Route Continuity:** The route must be connected from source to destination.
- **🚧 Exclusion of Unsafe Roads:** Roads that fail to meet safety thresholds (quality, drainage, flood depth) are removed.
- **🌍 Geospatial Flood Risk Zones:** Roads are categorized into **high, moderate, and low-risk zones**.

## 🏗️ Optimization Approaches
We implemented and compared two methods:

| Method | Pros | Cons |
|--------|------|------|
| **Exact Optimization (LP)** | ✅ Guarantees the safest possible route<br>✅ Best for **evacuations** | ❌ Computationally expensive<br>❌ Not scalable for large datasets |
| **Simulated Annealing** | ✅ Scalable & computationally efficient<br>✅ Suitable for **large networks & real-time routing** | ❌ Does not guarantee a globally optimal solution |

## 📂 Installation & Usage
### 🔧 Requirements
- Python 3.x
- Install dependencies:
  ```bash
  pip install numpy pandas matplotlib scipy pulp
