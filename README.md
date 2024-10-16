# EnRoute: Transit Navigator for Delhi Bus and Metro System

### Overview
EnRoute is a transit navigation system designed to help users find the shortest, most cost-effective, and least interchange-heavy routes through the Delhi Metro and bus systems. Using efficient data structures and algorithms, the platform provides an optimized travel experience.

### Key Features
- **Shortest Route Calculation**: Find the fastest and least costly route between two points.
- **Interchange Minimization**: Prioritizes routes with the fewest changes between metro lines or bus routes.
- **Real-Time Route Planning**: Includes real-time traffic and schedule data for accurate navigation.
- **Autocomplete Search**: Fast and responsive search for metro or bus stop names using a prefix tree (Trie).

### Technologies Used
- **Data Structures**:
  - Graph (Undirected Weighted Graph): For modeling the metro and bus network.
  - Adjacency List: Efficient space utilization for the network representation.
  - Hashmaps: For fast lookup of station details, routes, and fare information.
  - Trie (Prefix Tree): For the autocomplete system.
  - Min-Heap (Priority Queue): Used in Dijkstra’s algorithm for optimal pathfinding.

- **Algorithms**:
  - **Dijkstra's Algorithm**: For shortest path calculation.
  - **Bellman-Ford Algorithm**: For handling negative edge weights, such as fare adjustments or delays.
  - **Breadth-First Search (BFS)**: For minimizing interchanges between routes.

### Data Sources
- CSV data from the Delhi Metro Rail Corporation (DMRC), which includes metro and bus station details, routes, fares, timings, and transfer points.

### Graphical User Interface (GUI)
- Developed using **GTK+**, offering a simple, user-friendly interface where users can input start and destination points and view multiple route options.

### How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/enroute-transit-navigator.git
   cd enroute-transit-navigator
   ```

2. Install dependencies:
   ```bash
   sudo apt-get install gtk+3.0
   ```

3. Run the application:
   ```bash
   ./run-enroute
   ```

### Future Enhancements
- Integration of real-time traffic data.
- AI-based predictions for route efficiency.
- Multi-city transit networks.
- Features like live bus tracking and personalized travel suggestions.

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
