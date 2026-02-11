# Genetic Algorithms applied to National Parks Route Optimization (Argentina)

This project applies Genetic Algorithms (GA) to solve a combinatorial optimization problem analogous to the Traveling Salesman Problem (TSP), focused on minimizing travel distance between National Parks in Argentina.

The model integrates spatial data processing, evolutionary optimization, and interactive visualization using R and Shiny.

---

## Project Overview

This project addresses a classical optimization problem applied to territorial routing.

Given a set of National Parks and their geographic coordinates, the objective is to determine the visitation order that minimizes total travel distance.

Because the number of possible routes grows exponentially, a Genetic Algorithm is implemented as a heuristic search method suitable for large solution spaces.

The workflow is fully reproducible in RMarkdown and includes an interactive Shiny application.

---

## Analytical Value

The project demonstrates:

- Application of evolutionary algorithms to spatial problems  
- Optimization of territorial mobility scenarios  
- Integration of geospatial data with algorithmic modeling  
- Exploration of hyperparameters in heuristic optimization  
- Translation of mathematical modeling into interactive tools  

Although developed for modeling purposes, the approach is applicable to logistics, tourism planning, and route optimization problems.

---

## Data

- Source: Sistema de Información de Biodiversidad (SIB Argentina)  
- File: `areas_protegidas.xlsx`  
- Variables used:
  - Area_protegida  
  - Latitud  
  - Longitud  

Coordinates correspond to approximate reference locations and are used for modeling purposes only.

To reduce computational complexity, a random subset of parks is selected in each execution.

---

## Methodology

The workflow includes:

1. Data cleaning and transformation  
2. Construction of a geographic distance matrix using `geosphere::distGeo`  
3. Definition of total route distance function  
4. Construction of fitness function (distance minimization)  
5. Genetic Algorithm implementation using the `GA` package  
6. Extraction of optimal route and minimum distance  
7. Hyperparameter search (population size, mutation rate, crossover probability, generations)  
8. Cost simulation based on optimal distance  
9. Interactive geospatial visualization with Leaflet  

---

## Interactive Application

A Shiny application allows users to:

- Modify GA hyperparameters  
- Recalculate the optimal route dynamically  
- Visualize results on an interactive satellite map  
- Observe estimated travel costs  
- Explore distance results in real time  

---

## Cost Simulation

An exploratory cost model is included based on:

- Cost per kilometer  
- Base travel cost  

Values are illustrative and used for modeling purposes.

---

## Technologies and Tools

- R  
- RMarkdown  
- Shiny  
- GA  
- geosphere  
- leaflet  
- plotly  
- rnaturalearth  
- sf  

---

## Results

The project produces:

- Optimized visitation route  
- Minimum total travel distance  
- Interactive geospatial visualization  
- Hyperparameter comparison results  
- Cost estimation output  
- Reproducible HTML + Shiny application  

---

## How to Run

1. Clone the repository  
2. Ensure `areas_protegidas.xlsx` is in the root directory  
3. Open the `.Rmd` file  
4. Run as Shiny application or render to HTML  

---

## Skills Demonstrated

- Combinatorial optimization  
- Genetic Algorithms implementation  
- Hyperparameter tuning  
- Geospatial modeling  
- Distance matrix computation  
- Interactive mapping  
- Simulation modeling  
- Reproducible reporting  

---

## Author

Maria Marcela Gomez
