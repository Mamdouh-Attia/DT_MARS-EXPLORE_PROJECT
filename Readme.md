# 🪐 DT Mars Explore Project: Data Structures & Algorithms

![Project Status](https://img.shields.io/badge/status-active-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Language](https://img.shields.io/badge/language-C++-orange)

---

## 🌟 Overview

Welcome to the **DT Mars Explore Project**! This project is a hands-on showcase of advanced data structures and algorithms, simulating the management and exploration of Mars missions. The codebase is modular, well-documented, and designed for learning, experimentation, and extension.

---

## 🚀 Project Flow

1. **Initialization:** Load mission data and set up the Mars environment.
2. **Location & Resource Management:** Use graphs and trees to represent locations, paths, and resources.
3. **Simulation:** Run exploration tasks, manage rover movements, and allocate resources efficiently.
4. **Reporting:** Output mission results, statistics, and visualizations.

---

## 🧩 Why These Data Structures?

- **Graphs:** To model Mars locations and possible paths between them. Graphs allow efficient pathfinding (e.g., Dijkstra’s algorithm for shortest route).
- **Trees:** Used for hierarchical resource management and quick lookup of mission assets.
- **Queues:** Manage rover task scheduling (FIFO ensures fair task assignment).
- **Stacks:** Useful for backtracking in exploration (e.g., undoing moves).
- **Lists/Arrays:** Store mission logs and sequential data.

Each structure was chosen for its strengths in representing real-world exploration scenarios and optimizing performance.

---

## 📁 Project File Explanations

| File/Folder                | Purpose & Details |
|----------------------------|-------------------|
| `DT_MARS-EXPLORE_PROJECT.sln` | Solution file for easy IDE setup |
| `DT_MARS-EXPLORE/`         | Main source code folder |
| ├── `MarsGraph.h/.cpp`     | Graph implementation for Mars map, locations, and pathfinding |
| ├── `ResourceTree.h/.cpp`  | Tree structure for resource management |
| ├── `RoverQueue.h/.cpp`    | Queue for rover task scheduling |
| ├── `MissionStack.h/.cpp`  | Stack for backtracking and undo operations |
| ├── `main.cpp`             | Entry point, runs the simulation and ties modules together |
| └── ...                    | Additional helpers, models, and utilities |
| `Readme.md`                | This documentation file |

---

## ✨ Features

- Modular implementations of core data structures
- Realistic Mars exploration simulation
- Efficient algorithms for pathfinding, scheduling, and resource allocation
- Extensible for new missions and data
- Clear code comments and documentation

---

## 🛠️ Technologies Used

- C++ (main language)
- STL (Standard Template Library)
- Object-Oriented Design

---

## 📦 Getting Started

1. **Clone the repository:**
    ```bash
    git clone https://github.com/<your-username>/DT_MARS-EXPLORE_PROJECT-master.git
    cd DT_MARS-EXPLORE_PROJECT-master
    ```
2. **Open the solution in your IDE (e.g., Visual Studio, VS Code)**
3. **Build and run:**
    - For Visual Studio: Open `DT_MARS-EXPLORE_PROJECT.sln` and build.
    - For command line:
      ```bash
      g++ -o mars_explore DT_MARS-EXPLORE/main.cpp DT_MARS-EXPLORE/*.cpp
      ./mars_explore
      ```

---

## 💡 Example Usage

```cpp
#include "MarsGraph.h"
#include "RoverQueue.h"

MarsGraph marsMap;
marsMap.addLocation("Base Camp");
marsMap.addLocation("Crater Alpha");
marsMap.connect("Base Camp", "Crater Alpha", 5); // 5km path

RoverQueue roverTasks;
roverTasks.enqueue("Collect samples at Crater Alpha");

while (!roverTasks.isEmpty()) {
    std::string task = roverTasks.dequeue();
    std::cout << "Executing: " << task << std::endl;
}
```

---

## 📂 File Structure

```text
DT_MARS-EXPLORE_PROJECT-master/
│
├── DT_MARS-EXPLORE_PROJECT.sln   # Solution file
├── DT_MARS-EXPLORE/              # Source code and modules
│   ├── MarsGraph.h/.cpp
│   ├── ResourceTree.h/.cpp
│   ├── RoverQueue.h/.cpp
│   ├── MissionStack.h/.cpp
│   ├── main.cpp
│   └── ...
├── Readme.md                     # Project documentation
└── ...
```

---

## 👤 License

- Licensed under the MIT License

---

## 🤝 Contributing

Contributions, suggestions, and feedback are welcome! Feel free to fork the repo, open issues, or submit pull requests.

---

## 📝 Notes

- This project is for educational purposes and demonstrates best practices in data structures and algorithms.
- Designed for learning, experimentation, and extension.

---

> **Explore. Simulate. Learn. 🚀**
