# 🍽️ Restaurant Simulation (SimPy)

## Overview

This project implements a **discrete-event simulation** of a restaurant system using **SimPy (Python)**.

The simulation models the full customer journey—from arrival to departure—while tracking resource usage and system performance.

---

## Author

**Habiba Abouraya**

---

## Objectives

* Simulate a real-world restaurant system
* Model customer flow and resource usage
* Analyze system performance using metrics
* Apply discrete-event simulation techniques

---

## System Description

The restaurant includes:

* Tables (seating customers)
* Chefs (food preparation)
* Waitstaff (service & payment)
* Cooking stations

Customers go through the following stages:

1. Arrival (random interarrival time)
2. Waiting for table
3. Order taking
4. Cooking
5. Serving
6. Dining
7. Payment
8. Leaving

---

## Technologies Used

* **Language:** Python
* **Library:** SimPy
* **Concepts:**

  * Discrete Event Simulation
  * Resource Allocation
  * Queue Management

---

## Simulation Logic

* Customers arrive using **exponential distribution**
* Service times use:

  * Uniform distribution
  * Normal distribution
* Resources are modeled using `simpy.Resource`

Each event is logged with:

* Time
* Queue lengths
* Resource usage
* Waiting times

---

## Performance Metrics

The simulation calculates:

* Total customers served
* Average wait for table
* Average wait for food
* Average total time in system
* Average table occupancy time
* Chef utilization
* Waitstaff utilization

---

## Simulation Output

The system generates:

### Statistics

* Summary metrics for performance evaluation

### Event Log Table

Includes:

* Time
* Customer
* Event type
* Queue sizes
* Busy resources

(See example output in project files)

---

## How to Run

1. Install SimPy:

```bash id="u7k1s3"
pip install simpy
```

2. Run the simulation:

```bash id="2c6f3w"
python simulation.py
```

3. View results in console

---

## 📄 Documentation

See full report here:
[Project Report](docs/report.pdf)

---

## 🧠 Key Concepts Demonstrated

* Discrete-event simulation
* Resource scheduling
* Queueing systems
* Performance evaluation

---

