# Autonomous Logistics Pathfinding & ETA Predictor

#  Project Overview
This project simulates an **Intelligent Agent** designed for urban delivery logistics. The goal is to solve a real-world problem: finding the most efficient path for a delivery drone in a grid-based environment while predicting the delivery time based on historical traffic data.

The project bridges the gap between **Classical Symbolic AI** (Search Algorithms) and **Modern Statistical AI** (Machine Learning).

# Key Features
* Dynamic Grid Environment: A 10x10 map with randomized obstacles representing an urban landscape.
* Rational Pathfinding: Uses the **A* (A-Star) Algorithm**, an informed search strategy, to find the shortest path from start to finish.
* Predictive Analytics: A Linear Regression model that estimates the total delivery time by analyzing path length and real-time traffic density.
* Data Visualization: Real-time plotting of the agent's route using Matplotlib.

#  Syllabus Concepts Applied
This project was developed to demonstrate core outcomes from the **Introduction to AI and ML** course:

 1. Intelligent Agents 
The system is designed as a Goal-Based Rational Agent. It perceives its environment (the grid) and chooses the sequence of actions that minimizes its cost function.

 2. Problem Solving & Search 
I implemented **Informed Search** using the A* algorithm. 
* Heuristic (h(n)): Manhattan Distance was used to guide the search efficiently toward the goal.
* Cost Function (g(n)): Tracks the actual steps taken to ensure the path is truly the shortest.

 3. Machine Learning & Probability 
Beyond just finding a path, the agent uses **Statistical Decision Theory**. 
* Estimator: A Linear Regression model treats "Traffic Density" as a random variable to predict "Time."
* Data Representation: Inputs are handled as feature vectors, demonstrating the application of Linear Algebra in ML.

# Requirements
To run this simulation, you will need **Anaconda** or a Python environment with:
* `numpy`
* `matplotlib`
* `scikit-learn`

If you don't have them, install them via terminal/command prompt:


pip install numpy matplotlib scikit-learn

# How to Run
1. Clone this repository to your local machine.
2. Open the script in **Jupyter Notebook**, **Spyder**, or **VS Code**.
3. Run the cells to generate a random map, calculate the path, and see the ML-based time prediction.

