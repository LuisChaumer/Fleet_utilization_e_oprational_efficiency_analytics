# Fleet Utilization & Operational Efficiency Analysis 🚚📊

**Author:** Luis Chaumer  
**Role:** Data Analyst  
**Company:** Icar Services
**Tools:** Python, Pandas, NumPy, Matplotlib, Jupyter Notebook  
**Dataset:** Synthetic — 112,568 fleet trips (May 2024 → May 2025)

---

## 📘 Project Overview

This project analyzes **fleet utilization and operational efficiency** for a fictional logistics/transport company operating across **5 regions** over a **1-year period** (May 2024 to May 2025).

The dataset contains **112,568 simulated trips** from a fleet of **200 vehicles**, including trip durations, mileage, and idle behavior.  
The goal is to evaluate:

- How efficiently vehicles are being used  
- Whether specific regions overuse or underuse the fleet  
- How much idle time and unproductive mileage exists  
- Key operational bottlenecks  
- Optimization opportunities to reduce operational costs  

---

## 🎯 Project Objectives

- Calculate key fleet KPIs:
  - **Utilization rate**
  - **Trip duration distribution**
  - **Mileage efficiency**
  - **Idle time patterns**
- Compare performance across **5 regions**
- Identify underused or overworked vehicles
- Detect operational inefficiencies that drive cost
- Provide actionable business recommendations  

---

## 📊 Dataset Description

The dataset contains **112,568 rows**, each representing a fleet trip:

| Column | Description |
|--------|-------------|
| `trip_id` | Unique trip identifier |
| `vehicle_id` | One of 200 vehicles (VH-001 → VH-200) |
| `region` | North, South, East, West, Central |
| `start_time` | Timestamp trip started |
| `end_time` | Timestamp trip ended |
| `duration_min` | Trip duration in minutes (5–180 min) |
| `mileage_km` | Distance traveled (km) |
| `idle_after_min` | Idle time after trip before next use |

Data reflects realistic fleet behavior via exponential & uniform distributions.

---

## 📈 Exploratory Analysis

### **1. Trip Duration Distribution**
![Trip Duration](images/trip_duration.png)

---

### **2. Mileage Distribution**
![Mileage](images/mileage_distribution.png)

---

### **3. Idle Time After Trips**
![Idle Time](images/idle_distribution.png)

---

### **4. Trips by Region**
![Trips by Region](images/trips_by_region.png)

---

## 🔍 Operational Insights

### ✦ **Trip Duration**
- Most trips fall between **15–60 minutes**, suggesting short-haul operations.
- A smaller tail of long trips (120–180 min) indicates occasional long-distance tasks.

### ✦ **Mileage Efficiency**
- Mileage correlates strongly with trip duration (expected).
- Vehicles used for short repetitive routes may be overscheduled.

### ✦ **Idle Time**
- Idle time distribution is wide:
  - Many vehicles idle < 30 minutes (high utilization)
  - A long tail up to 600 minutes highlights underused vehicles
- Idle spikes may indicate:
  - Poor dispatching  
  - Region imbalance  
  - Bottlenecks in routing  

### ✦ **Regional Distribution**
- Trip volume per region reveals operational load and resource imbalance.
- Overloaded regions may require:
  - Fleet reallocation  
  - Shift restructuring  
  - Additional staffing  

---

## 🚀 Business Recommendations

### ✔️ 1. Rebalance Fleet Allocation  
Regions with high trip volumes and low idle time should receive more vehicles.  
Underused regions show opportunity to **move fleet resources**.

### ✔️ 2. Reduce Idle Time  
Vehicles showing frequent high idle periods may require:
- Better route scheduling  
- Redistributed workloads  
- Automation in dispatching  

### ✔️ 3. Monitor Long-Haul Trips  
Long trips (>120 min) may:
- Require different maintenance cycles  
- Consume more fuel  
- Need specialized drivers  

### ✔️ 4. Optimize Overlapping Routes  
Repeated short-distance patterns suggest:
- Inefficient routing  
- Missed opportunities to cluster deliveries  

### ✔️ 5. Build Fleet KPIs Dashboard  
Include:
- Utilization rate  
- Idle time heatmap  
- Trips per region  
- Mileage per vehicle  
- Underused/overused vehicle ranking  

(This project can later be transformed into a full dashboard.)

---

## 🧰 Tech Stack

- **Python:** Pandas, NumPy, Matplotlib  
- **Data Structure:** Fleet trips synthetic dataset  
- **Notebook:** Jupyter Notebook  
- **KPIs:** Utilization, idle distribution, mileage efficiency  

---

## 📁 Repository Structure

fleet-utilization-analysis/
├── data/
│ └── fleet_utilization_dataset.csv
├── images/
│ ├── trip_duration.png
│ ├── mileage_distribution.png
│ ├── idle_distribution.png
│ └── trips_by_region.png
├── notebooks/
│ └── fleet_analysis.ipynb
└── README.md

yaml
Copiar código

---

## 📬 Contact

**Luis Chaumer**  
Data Analyst  
📩 Email: luischaumer@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/luis-chaumer123  
