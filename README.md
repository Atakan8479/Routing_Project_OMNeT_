# 🚦 Routing Project in OMNeT++

This project explores and implements enhanced routing mechanisms in OMNeT++ for both educational and performance-focused simulations. It introduces centralized routing, FSM simplifications, and performance tracking to improve packet delivery efficiency and provide deeper insights into network behavior.

---

## 🧠 What is OMNeT++?

[OMNeT++](https://omnetpp.org) is a modular, component-based C++ simulation environment widely used for academic research and network simulation. It supports:

- Graphical Eclipse-based IDE  
- The NED language for defining network structures  
- Hierarchical and reusable model design  
- Real-time visualization and statistics tracking  
- Extensions through INET, Simu5G, Veins, etc.

In this project, OMNeT++ was used to model custom routing protocols and evaluate them in various topologies using detailed performance metrics.

---

## 🎯 Project Objective

- Develop and refine routing strategies  
- Enable centralized routing logic with toggleable configuration  
- Compare simulation performance across static topologies  
- Reduce packet loss and delay while improving throughput  
- Visualize and analyze collected metrics using Python tools

---

## ⚙️ Key Features

- ✅ Centralized routing parameter toggle (`centralRouting`)
- ✅ FSM-based application optimization (BurstyApp.cc)
- ✅ Static routing via `cTopology`  
- ✅ Dynamic metric collection (latency, hops, throughput)  
- ✅ Lightweight message broadcasting & route serialization  
- ✅ Scenario-based configuration for multi-topology support

---

## 🌐 Network Scenarios

The project includes multiple test topologies for benchmarking:

- **Net5**: Simple 5-node testbed for feature validation  
- **Net60**: Large-scale, stress-test topology with cut-through and store-and-forward modes  
- **RandomMesh / Mesh**: For variability and adaptive behavior evaluation

---

## 📊 Tracked Metrics

The simulation tracks and compares:

- 📦 Packet Delivery Ratio  
- ⏱ End-to-End Delay  
- 🧮 Queue Utilization  
- 📈 Throughput  
- ❌ Packet Loss  

All metrics are exported and visualized via Python/Colab notebooks.

---

## 🛠 Technologies Used

- **OMNeT++** (6.x recommended)  
- **INET Framework**  
- **C++ / NED** (for logic and topology files)  
- **Python + Matplotlib** (for post-simulation analysis)  
- **Google Colab** (optional result visualization)

---

## 🗂 Project Structure

```bash
Routing_Project_OMNeT_/
│
├── src/                    # Core C++ routing and app modules
│   ├── routing/            # Centralized routing logic
│   └── application/        # FSM-based traffic generation
│
├── ned/                    # Network description files (NED)
│   ├── topologies/         # Net5, Net60, Mesh, etc.
│   └── config/             # Parameters, modules
│
├── results/                # Scalar/vector output from simulations
│
├── analysis/               # Python notebooks and CSV evaluation
├── omnetpp.ini             # Scenario & runtime configuration
└── README.md               # Project overview
