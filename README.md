# EECS 281 Projects - Data Structures and Algorithms

I developed a series of complex software projects as part of **EECS 281**, an undergraduate course at the University of Michigan focusing on **data structures** and **algorithms**. These projects involved solving real-world problems by implementing advanced algorithms and optimizing data structures for efficiency.

### Projects and Data Structures Used:

1. **2D and 3D Environments and Puzzles**  
   - **Data Structures Used:** Graphs (adjacency lists), Queues, Stacks  
   - **Description:** Utilized graphs for route tracing in 2D and 3D environments, leveraging **Breadth-First Search (BFS)** and **Depth-First Search (DFS)** for puzzle-solving.

2. **Zombie Tower Defense**  
   - **Data Structures Used:** Priority Queues, Templated Containers, Inheritance, Interface Programming  
   - **Description:** Implemented **priority queues** to manage task execution in a game simulation, working with **templated containers** and applying **object-oriented principles** like inheritance and interfaces.

3. **Bank Simulation**  
   - **Data Structures Used:** Hash Tables  
   - **Description:** Employed **hash tables** for efficient data retrieval in a banking system simulation, managing account data and transactions.

4. **Zoo Optimization Algorithms**  
   - **Data Structures Used:** Dynamic Programming Tables, Custom Containers  
   - **Description:** Worked with **dynamic programming** and **custom containers** to solve optimization problems such as the **Traveling Salesperson** and **Knapsack problem**.

### Disclaimer:

In compliance with the University of Michigan's honor code, I cannot publicly share the source code. However, please contact me if you would like to look at the project code. A detailed descriptions of each project’s key functionalities and the technical concepts applied are provided above to highlight my technical expertise and problem-solving skills.

# Project 1: Pathfinding and Search Algorithms

This project, part of the EECS 281 course at the University of Michigan, involved developing a pathfinding solution using advanced data structures and algorithms. The objective was to simulate a search algorithm that could navigate through a map, identify specific points (like start and end locations), and backtrack or find valid paths based on specific constraints. The project focused on designing efficient algorithms for traversal using a variety of data structures including queues, stacks, and maps.

## Key Features

- **Pathfinding Implementation:**  
  Using breadth-first search (queue-based) or depth-first search (stack-based), the program simulates pathfinding on a 2D grid, considering obstacles and boundaries.
  
- **Custom Data Structures:**  
  The project leverages custom containers and a deque-based backtrace mechanism to explore possible paths dynamically.

- **Flexible Map Representation:**  
  The program allows for dynamic maps with different dimensions, handling multiple character symbols (for obstacles, starting points, and goals) in the map grid.

- **Multi-color and Symbol Support:**  
  The system can handle maps with multiple color schemes for varied search configurations, such as identifying and distinguishing between different types of paths and obstacles.

- **Mode Selection:**  
  The project includes an option for users to choose between different search strategies (stack vs queue), offering flexibility in how the search algorithm explores the map.

- **Backtracking and State Management:**  
  The project incorporates backtracking and state-checking mechanisms to ensure that already explored paths are not revisited, improving efficiency.

## Technologies Used

- C++
- Standard Library: `deque`, `unordered_set`, `vector`, `queue`, `stack`, `map`, etc.
- Custom Data Structures for Pathfinding

## Project Highlights

This project demonstrates proficiency in graph traversal, data structure manipulation, and problem-solving techniques, reflecting the application of data structures like deques, stacks, and unordered sets to manage search states and paths effectively.

# Project 2: Dynamic Memory Management

## Overview

This project, part of the **EECS 281** course at the **University of Michigan**, focuses on simulating dynamic memory allocation and deallocation strategies. The objective is to develop a memory management system that simulates the allocation of memory blocks during runtime using strategies such as **first-fit**, **best-fit**, and **worst-fit**. Additionally, the project includes a garbage collection simulation and visualizes the impact of memory fragmentation on system performance.

## Key Features

- **Dynamic Memory Allocation**  
  Simulates dynamic memory allocation where memory blocks of various sizes are allocated and deallocated based on the selected strategy (first-fit, best-fit, worst-fit).
  
- **Memory Block Management**  
  Utilizes custom memory blocks and free lists to manage memory and track available free space, improving memory reuse and minimizing fragmentation.

- **Garbage Collection Simulation**  
  Implements a basic garbage collection mechanism to identify unused memory and free it for future allocations.

- **Fragmentation Visualization**  
  Visualizes memory fragmentation as allocations and deallocations occur, showing the effects of different memory strategies on system performance.

- **Memory Management Strategies**  
  Allows users to choose between **first-fit**, **best-fit**, and **worst-fit** allocation strategies and observe their impact on memory usage and fragmentation.

- **Performance Monitoring**  
  Provides feedback on memory usage and fragmentation in real-time, helping users understand the efficiency of each allocation strategy.

## Technologies Used

### C++ Programming Language

The project is implemented in C++, utilizing its memory management capabilities to simulate dynamic allocation and deallocation.

### Standard Library

Utilizes C++ Standard Library components such as:
- **`vector`**: To manage dynamic arrays of memory blocks.
- **`list`**: Used for managing free memory blocks and allocation order.
- **`map`**: Helps efficiently track and organize allocated blocks and free memory lists.

### Custom Data Structures

Custom data structures are implemented to efficiently manage free memory blocks and simulate memory allocation strategies. These include:
- **Free List**: A custom data structure for managing the pool of available memory blocks.
- **Memory Block**: A structure representing individual memory units within the simulation.

## Project Highlights

This project compares memory allocation strategies (first-fit, best-fit, worst-fit) and utilizes custom data structures like free lists for efficient memory management. It includes real-time visualization of memory fragmentation, offering insights into how different strategies impact memory usage and system performance.

# Project 4: Traveling Salesman Problem (TSP) and Minimum Spanning Tree (MST) Algorithms

This project implements algorithms to solve two classic problems in graph theory: the **Traveling Salesman Problem (TSP)** and the **Minimum Spanning Tree (MST)**. These problems are fundamental in various applications, including logistics, network design, and optimization.


## Introduction
The project solves two important graph problems:
- **Minimum Spanning Tree (MST)**: Connects all vertices in a graph with the minimum possible total edge weight, avoiding cycles.
- **Traveling Salesman Problem (TSP)**: Finds the shortest possible route that visits each vertex exactly once and returns to the starting point.

## Algorithms

### Minimum Spanning Tree (MST)
The MST is solved using **Prim's Algorithm**, which:
- Starts from an arbitrary vertex.
- Expands the tree by adding the minimum weight edge that connects a new vertex to the tree.
- Continues until all vertices are included in the tree.
  
### Traveling Salesman Problem (TSP)
TSP is solved using multiple approaches:
- **Greedy Algorithm (FastTSP)**: A heuristic approach that picks the nearest unvisited vertex at each step to approximate the optimal solution.
- **Backtracking with Branch and Bound (OPTTSP)**: An exact method that systematically explores all possible routes to find the shortest possible tour. It uses pruning techniques to eliminate suboptimal solutions.
- **2-opt Optimization**: An improvement on an existing TSP tour that eliminates crossing paths, refining the solution to reduce the total distance traveled.

## Technologies Used
- **Programming Language**: C++
  - Chosen for its performance in handling large datasets and complex algorithms efficiently.
- **Euclidean Distance**: Used to calculate the distance between vertices for the TSP problem.
- **Data Structures**: Custom data structures (e.g., vectors, queues) are used to efficiently manage vertices and edges.

## Applications
- **Network Design**: The MST algorithm is used to design cost-effective communication or transportation networks by connecting a set of nodes with the minimum total cost.
- **Logistics Optimization**: The TSP algorithm is crucial for optimizing routes in transportation and delivery services.
- **Computational Geometry**: Both algorithms are fundamental in geometric optimizations, such as efficient pathfinding and resource allocation.

## Project Highlights

The project demonstrates key optimization techniques for solving TSP and MST, offering both heuristic and exact methods for finding solutions, and sets the foundation for future developments like scalability and parallel computation in large-scale instances.

## Acknowledgements

Special thanks to University of Michigan, my teammates and the EECS281 staffs for providing the resources and environment to build these application.











