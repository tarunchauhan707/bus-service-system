# City Bus Service Simulation

This project simulates a city bus service using a graphical representation of the city map. The program allows users to select the source and destination points and provides the shortest path based on the selected criteria: minimum time, minimum cost, or traveling to all cities.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Contributing](#contributing)
- [License](#license)

## Overview

This C++ program utilizes several libraries, including `graphics.h`, to visually represent a city map and simulate a bus service. The program allows users to choose between different criteria for the journey and calculates the shortest path accordingly.

## Features

- **Graphical Representation:** Displays a city map with nodes representing different locations.
- **Shortest Path Calculation:** Calculates the shortest path based on user-selected criteria (minimum time or minimum cost).
- **Visualization:** Animates the movement of the bus along the calculated path.

## Getting Started

### Prerequisites

- Turbo C++ or any compatible IDE with support for `graphics.h`.

## Usage

1. Compile and run the `main` function.
2. Follow the on-screen instructions to select the source and destination points.
3. Choose the desired criteria for the journey:
   - Minimum time
   - Minimum cost
   - Traveling to all cities

## Code Explanation

### Libraries
- `graphics.h`: For graphical functions.
- `dos.h`: For delay function.
- `string.h` and `ctype.h`: For string and character handling functions.

### Main Components

- **Graph Representation:** The city map is represented as a graph with a 2D array `a[V][V]`, where `V` is the number of vertices.
- **Shortest Path Calculation:** The `algo` function implements Dijkstra's algorithm to find the shortest path based on the selected criteria.
- **Graphical Functions:** The `fun` function animates the bus movement, and the `welcome_screen` function displays the welcome message.
- **Utility Functions:** Includes functions like `minDistance` to find the vertex with the minimum distance, `printSolution` to display the results, and `prin` to convert vertex indices to characters.

#### Dijkstra's Algorithm:

-**int minDistance(int dist[], int sptSet[]):** Finds the vertex with the minimum distance that is not yet included in the shortest path tree.
-**void printSolution(int parent[], int n, int graph[V][V], int des, int time[V][V], int c):** Prints the solution and draws the final route.
-**void algo(int graph[V][V], int src, int des, int time[V][V], int c):** Implements Dijkstra's algorithm to find the shortest path from the source to the destination.

