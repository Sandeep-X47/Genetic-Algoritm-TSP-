---

# **Genetic Algorithm for Solving the Travelling Salesman Problem (TSP)**

This project implements a **Genetic Algorithm (GA)** to solve the **Travelling Salesman Problem (TSP)**, a classic optimization problem. The goal is to find the shortest possible route that visits a set of cities and returns to the starting city. 

## **Key Concepts:**

- **Genetic Algorithm (GA)**: An evolutionary optimization technique inspired by natural selection, where the fittest individuals are selected to produce offspring for the next generation. Over time, solutions evolve toward better routes.
  
- **Travelling Salesman Problem (TSP)**: A combinatorial optimization problem where the objective is to find the shortest path through a set of cities, visiting each city once and returning to the starting point.

## **Features:**

- **Fitness Evaluation**: Routes are evaluated based on their total distance. Shorter routes have higher fitness.
- **Selection**: Uses a **Roulette Wheel** selection method to choose the best individuals (routes) for reproduction.
- **Crossover**: Implements **Ordered Crossover (OX)** to combine two parent routes and produce new offspring.
- **Mutation**: Introduces diversity by swapping cities randomly in a route with a set **mutation rate**.
- **Visualization**: Uses **matplotlib** to visually represent the cities and the best route found by the algorithm.

## **Libraries Used:**
- `random`: For generating random routes, selections, and mutations.
- `numpy`: For efficient numerical computations, including calculating distances between cities.
- `matplotlib`: For plotting and visualizing the best route.

## **How It Works:**
1. **Population Initialization**: A random set of routes is created.
2. **Fitness Calculation**: Each route is evaluated based on its total distance.
3. **Selection**: The best routes are selected based on their fitness.
4. **Crossover & Mutation**: Selected routes are combined and mutated to form a new population.
5. **Generational Evolution**: The algorithm iterates over multiple generations to improve the population.
6. **Result**: The shortest route is found and visualized.

## **How to Run:**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/genetic-algorithm-tsp.git
   cd genetic-algorithm-tsp
   ```
2. Install dependencies:
   ```bash
   pip install numpy matplotlib
   ```
3. Run the script:
   ```bash
   python tsp_genetic_algorithm.py
   ```

## **Visual Output:**
The final output includes a plot of the cities and the optimal route found by the Genetic Algorithm.

## **Future Improvements:**
- Explore different selection techniques (e.g., tournament selection).
- Implement alternative crossover and mutation strategies.
- Support for larger datasets and more complex optimizations.

---
