Flood-Aware Routing Optimization for Jeddah’s Rainy Days
Authors:

Aseel A. Allmehmadi – Department of Computer Science and Engineering, University of Jeddah (2211696@uj.edu.sa)
Hadeel A. Sirdar – Department of Computer Science and Engineering, University of Jeddah (2210937@uj.edu.sa)
Fatima A. Almaashi – Department of Computer Science and Engineering, University of Jeddah (2210392@uj.edu.sa)
Overview

Jeddah, Saudi Arabia, is prone to severe flooding due to its unique topographical features and rapid urban expansion. This project develops an optimization model for flood-aware routing, improving urban resilience by ensuring safer transportation routes during floods.

We implemented two optimization techniques:

Exact Optimization (Linear Programming) for high-precision, small-scale problems.
Simulated Annealing for near-optimal solutions with better scalability for large-scale networks.
Methodology

The optimization problem is formulated to maximize route safety by considering:

Road Quality (q)
Drainage Efficiency (e)
Flood Depth (d)
Each road segment is evaluated based on a safety score, and constraints ensure:

Route continuity
Exclusion of unsafe roads (based on quality, drainage efficiency, and flood depth thresholds)
The project uses geospatial flood risk maps to classify Jeddah into high, moderate, and low-risk zones.

Optimization Approaches
Exact Optimization (Linear Programming)
Guarantees the safest possible route.
Best for small-scale or critical evacuation scenarios.
Computationally expensive for large networks.
Simulated Annealing
Provides a near-optimal solution in significantly less time.
Suitable for real-time, large-scale routing.
Balances accuracy with computational efficiency.
Installation

Requirements
Python 3.x
Required libraries:
pip install numpy pandas matplotlib scipy pulp
Clone the Repository
git clone https://github.com/yourusername/FloodAwareRouting.git
cd FloodAwareRouting
Run the Optimization
Execute the Jupyter Notebook:

jupyter notebook Flood-Aware Routing Optimization.ipynb
Dataset

The dataset used for this study includes flood risk zones and road network data.
Located in datasets_small_large.xlsx.
Results & Analysis

Exact Optimization works best for small-scale evacuation planning.
Simulated Annealing is effective for large-scale, real-time applications.
Future improvements include:
Integration with real-time weather and traffic data.
Machine learning-based flood prediction models.
Development of a public-facing application for real-time route guidance.
