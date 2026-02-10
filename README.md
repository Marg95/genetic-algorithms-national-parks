# Genetic Algorithms for Optimized Routes in Argentine National Parks

## Project Overview

This project applies **Genetic Algorithms (GA)** to solve a combinatorial optimization problem analogous to the **Traveling Salesman Problem (TSP)**, focusing on finding an optimal travel route between **National Parks in Argentina**.

The objective is to **minimize the total travel distance** between selected parks using evolutionary optimization techniques, while providing an interactive spatial visualization and cost simulation.

---

## Objectives

- Model a route optimization problem using Genetic Algorithms
- Minimize total travel distance between national parks
- Explore the impact of GA hyperparameters on solution quality
- Visualize optimized routes using interactive maps
- Simulate travel costs based on optimized distances
- Provide an interactive Shiny application for exploration

---

## Data Source

The dataset of protected areas was obtained from the **Sistema de Información de Biodiversidad (SIB)**:  
https://sib.gob.ar/listado_parques.php?accion=parques

**Important note:**  
Geographic coordinates are approximate and used for **educational and modeling purposes only**, not for real-world navigation.

---

## Methodology

1. **Data Cleaning and Preparation**
   - Removal of metadata rows
   - Selection of park names and geographic coordinates
   - Conversion of coordinates to numeric format

2. **Distance Matrix Construction**
   - Geographic distances computed using the `distGeo()` function from the `geosphere` package
   - Distances expressed in kilometers

3. **Genetic Algorithm Optimization**
   - Each individual represents a permutation of park visit order
   - Fitness function defined as the negative total route distance
   - GA operators:
     - Selection
     - Crossover
     - Mutation
   - Hyperparameter tuning through randomized search

4. **Route Optimization Output**
   - Optimal route sequence
   - Minimum total travel distance

---

## Visualization

- Interactive **Leaflet map** showing:
  - National and provincial boundaries
  - National park locations
  - Optimized travel route
- Visual support for spatial interpretation of the algorithm results

---

## Cost Simulation

A simplified travel cost simulation is included, based on:
- Average cost per kilometer
- Fixed base cost for park access and general expenses

**Disclaimer:**  
All cost values are hypothetical and intended for **illustrative purposes only**.

---

## Interactive Application (Shiny)

A Shiny application allows users to:
- Adjust GA hyperparameters in real time
- Recompute optimized routes
- Visualize updated routes on an interactive map
- Observe changes in distance and estimated costs

---

## Technologies Used

- R
- Genetic Algorithms (`GA` package)
- Leaflet (interactive maps)
- Geosphere (geographic distance calculations)
- Shiny (interactive application)
- Plotly (interactive visualization)

---

## Author

Maria Marcela Gomez
