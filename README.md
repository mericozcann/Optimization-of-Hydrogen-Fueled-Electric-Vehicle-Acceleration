# Optimization Study of Hydrogen Fueled Electric Vehicle Acceleration
This project focuses on optimizing vehicle acceleration and energy consumption for a hydrogen-powered electric city vehicle, particularly for the Shell Eco-marathon competition. The optimization includes vehicle parameters such as torque, wheel diameter, and speed, taking into account motor efficiency, regenerative braking, and different driving profiles.

## Table of Contents
1. Project Overview
2. Installation
3. Usage
4. Optimization and Simulation
5. Results
6. Requirements

## Project Overview
This project aims to optimize the performance of a hydrogen-powered vehicle by:

* Maximizing acceleration while minimizing energy consumption.
* Incorporating regenerative braking.
* Simulating different driving profiles (urban and highway) to assess vehicle performance under various conditions.
* Using Monte Carlo simulations to analyze average and standard deviations of acceleration.
* Performing Sobol sensitivity analysis to identify key parameters that affect vehicle performance.
The main optimization parameters are:

* Torque (Nm)
* Wheel Diameter (m)
* Speed (km/h)

## Installation
To run this project, you will need to install the required Python libraries. You can install the necessary packages using pip:

pip install numpy pandas matplotlib scipy SALib

## Usage
1. Clone the repository and navigate to the project folder:

git clone https://github.com/yourusername/vehicle-optimization.git
cd vehicle-optimization

2. Run the Python file that contains the optimization model:

python vehicle_optimization.py

### Running the Simulation
The script will automatically run the following steps:

* Calculate the optimal torque, wheel diameter, and speed using differential evolution optimization.
* Simulate urban and highway driving profiles.
* Run a Monte Carlo simulation for performance variability.
* Perform Sobol sensitivity analysis.
The results, including acceleration and energy consumption, will be printed to the console.

## Optimization and Simulation
### Vehicle Parameters
The initial vehicle parameters are defined as follows:

* Mass: 140 kg
* Wheel Diameter: 0.5 m
* Motor Power: 20 kW
* Torque: 200 Nm
* Aerodynamic Drag Coefficient: 0.3
* Battery Capacity: 5.5 kWh
* Air Resistance: 1.2 kg/m³
* Frontal Area: 1.6 m²
* Rolling Resistance: 0.015

### Monte Carlo Simulation
The project includes a Monte Carlo simulation to analyze the average acceleration and standard deviation based on random variations in torque, wheel diameter, and speed. The simulation is run with 1024 samples.

### Sobol Sensitivity Analysis
Sobol sensitivity analysis is performed to evaluate the impact of torque, wheel diameter, and speed on the optimization outcome.

## Results
The script provides the following results:

* Optimal Torque: 150.00 Nm
* Optimal Wheel Diameter: 0.70 meters
* Optimal Speed: 100.00 km/h
* Average Acceleration: -0.59 m/s²
* Standard Deviation: 5.77 m/s²

### Sensitivity Analysis Results:
* Torque sensitivity: 0.0096
* Wheel Diameter sensitivity: 0.0518
* Speed sensitivity: 0.9365

## Requirements
* Python 3.8 or higher
* Numpy
* Pandas
* Matplotlib
* Scipy
* SALib
