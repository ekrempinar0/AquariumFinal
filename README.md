# AquariumFinal

AquariumFinal
Project Overview

This project is a computational simulation designed to predict biological and chemical changes in a closed aquarium ecosystem over a 30-day period. Real-world biological processes, such as photosynthesis and waste accumulation, are represented in a simplified mathematical framework to visualize how the system evolves over time.

Mathematical Model

The aquarium system is described using equations that track the rate of change of key chemical variables, including Oxygen (O₂), Carbon Dioxide (CO₂), and Ammonia (NH₃). These variables are updated at discrete time intervals to represent daily changes within the ecosystem.

Biological Components

Algae (Producers):
Algae act as oxygen producers through photosynthesis and consume carbon dioxide in the process. The efficiency of oxygen production depends on light conditions and the amount of algae present in the system.

Fish (Consumers):
Fish consume oxygen for respiration and release ammonia and carbon dioxide as metabolic waste. As the fish population increases, oxygen consumption and waste production increase accordingly.

Light Efficiency

Photosynthetic efficiency is controlled by a light efficiency coefficient, which represents how well different light types support photosynthesis:

Purple Light: High efficiency due to strong absorption by chlorophyll

White Light: Moderate efficiency with a balanced spectrum

Green Light: Low efficiency because most green light is reflected rather than absorbed

This coefficient directly influences the rate of oxygen production by algae.

Numerical Method – Euler Approach

The system is solved using a discrete-time numerical method based on Euler’s Method. At each time step, the future state of the system is calculated using the current state and the net effect of biological production and consumption processes.

This approach allows the system to evolve dynamically while keeping the numerical implementation simple and transparent.

System Constraints and Survival Logic

Ammonia Toxicity:
When ammonia levels become too high, the environment turns toxic and fish mortality increases.

Mechanical Stress:
Prolonged operation of the filtration system at high power creates mechanical stress, which negatively affects fish survival.

These constraints ensure that the simulation reflects realistic ecological limits.

# Ecosystem Simulation Project


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WF8CPHUWUtMgVpoh0rWMCG2e1IvbOMnY#scrollTo=q1w19gk2q3Sj)

