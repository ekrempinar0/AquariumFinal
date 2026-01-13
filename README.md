# AquariumFinal

1. Project Overview
This project is a computational simulation designed to predict biological and chemical changes in a closed aquarium ecosystem over a 30-day period. It translates real-world biological phenomena, such as the nitrogen cycle and photosynthesis, into a mathematical model to visualize system behavior over time.


2. Mathematical Model
The system is modeled using equations that describe the rate of change for Oxygen (O2), Carbon Dioxide (CO2), and Ammonia (NH3).

Biological Components:

Algae (Producers): The rate of O2 production and CO2 consumption is scaled by a light efficiency coefficient (Epsilon).
O2 Production = Algae Count × 0.6 × Epsilon
CO2 Consumption = Algae Count × 0.4 × Epsilon

Fish (Consumers): Fish consume O2 and produce NH3 and CO2 as metabolic byproducts.
O2 Consumption = Fish Count × 0.5
NH3 Production = Fish Count × 0.25

Light Efficiency Coefficients (Epsilon): Coefficients are assigned based on the chlorophyll absorption spectrum to represent photosynthetic efficiency:

Purple Light: Epsilon = 2.5 (Maximum absorption peak).

White Light: Epsilon = 1.0 (Balanced spectrum).

Green Light: Epsilon = 0.1 (Minimum efficiency due to reflection).

3. Numerical Method: The Euler Approach
To solve these equations dynamically, we implemented a Discrete-Time Update Method (Euler’s Method). The state of the system at each daily step (t + 1) is calculated based on its state at time t.

The General Update Formula:
Future State = Current State + (Production Rate - Consumption Rate) × Time Step

4. System Constraints & Survival Logic

Ammonia Toxicity: If NH3 levels exceed 80 units, the environment becomes toxic, causing daily fish fatalities.

Mechanical Stress: If the filter power is set to "High" for more than 5 consecutive days, the resulting stress leads to fish death every 2 days.


# Ecosystem Simulation Project

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Q_JtmlwyK4qgSNat7VZOovm6bJOqZEwa?usp=sharing)
