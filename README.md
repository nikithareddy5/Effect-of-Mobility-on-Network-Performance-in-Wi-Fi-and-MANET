# Effect-of-Mobility-on-Network-Performance-in-Wi-Fi-and-MANET

## Project Overview

This project analyzes the performance of a **Mobile Ad Hoc Network (MANET)** under different node mobility speeds.
The simulation evaluates how increasing node speed impacts key network performance metrics such as:

* **Throughput**
* **Packet Delivery Ratio (PDR)**
* **End-to-End Delay**

The goal of this study is to understand how mobility affects network reliability and efficiency in dynamic wireless environments.

---

## Technologies Used

* **NS-3 Network Simulator**
* **C++** for simulation implementation
* **Python (Matplotlib)** for visualization
* **Data Analysis & Plotting**

---

## Project Structure

```
MANET-Performance-Analysis
│
├── manet_project.cc        # NS-3 simulation code
├── plots_manet.py          # Python script to generate graphs
├── results/
│   ├── throughput_plot.png
│   ├── pdr_plot.png
│   ├── delay_plot.png
│
└── README.md
```

---

## Simulation Description

The network simulation evaluates MANET performance by varying **node speed from 1 m/s to 25 m/s**.

For each speed, the following metrics are recorded:

| Metric                          | Description                                               |
| ------------------------------- | --------------------------------------------------------- |
| **Throughput**                  | Amount of data successfully transmitted per second (kbps) |
| **Packet Delivery Ratio (PDR)** | Percentage of packets successfully received               |
| **End-to-End Delay**            | Average time taken for packets to reach the destination   |

---

## Results

### Throughput vs Node Speed

Higher throughput indicates efficient data transmission.

* Throughput remains **high at lower speeds**
* Drops significantly at **higher mobility levels**

---

### Packet Delivery Ratio (PDR)

PDR measures network reliability.

* **~98% PDR at low speeds**
* Drops as node mobility increases
* High mobility leads to **frequent route breakages**

---

### End-to-End Delay

Average packet delivery delay increases with mobility.

* Low delay at **stable node speeds**
* Higher delays when **network topology changes rapidly**

---

## Performance Observations

Key insights from the simulation:

* **Low mobility improves network stability**
* **High node speed decreases packet delivery**
* **Network delay increases with mobility**
* MANET routing protocols must handle **frequent topology changes**

---

## Visualization

The project includes Python-generated plots for:

* Speed vs Throughput
* Speed vs Packet Delivery Ratio
* Speed vs Average End-to-End Delay

These visualizations help identify how **mobility impacts network performance**.

---

## How to Run the Project

### 1. Run the NS-3 Simulation

Compile and run the simulation file:

```
./waf --run manet_project
```

---

### 2. Generate Graphs

Run the Python visualization script:

```
python3 plots_manet.py
```

This will generate performance graphs for the simulation results.

---

## Applications

Understanding MANET performance is useful for:

* Emergency communication systems
* Military communication networks
* Disaster recovery networks
* Vehicular ad hoc networks (VANETs)

---

## Future Improvements

Possible extensions to this project:

* Compare multiple routing protocols (AODV, DSR, OLSR)
* Simulate larger network sizes
* Evaluate packet loss and jitter
* Introduce realistic mobility models

---


**Nikita Baddam**


