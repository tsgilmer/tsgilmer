My name is Tyler "Slade" Gilmer, and I am a graduate student at the University of Alabama in Huntsville, majoring in Industrial and Systems Engineering.

I design and build data-driven decision systems for complex, disruption-prone environments, focusing on manufacturing systems and infrastructure networks.

My work combines simulation, machine learning, and systems modeling to improve resilience, efficiency, and operational decision-making.

---

## Featured Projects

# American Heartland Rail System

## 📄 Final Paper

(American%20Heartland%20Rail%20Final.pdf)

## 📊 Overview

This project presents a phased, economically viable intercity rail network for the U.S. Midwest and South. The model evaluates ridership, revenue, and benefit-cost ratios across multiple corridor configurations using simulation and economic analysis.

## 🔧 Methods

* Network modeling (Python / NetworkX)
* Gravity-based demand modeling
* Monte Carlo simulation
* Cost-benefit and BCR analysis

## 📈 Key Results

* Strong BCR (>2.0 in base case)
* Robust performance across sensitivity scenarios
* Identified high-impact corridors (Chicago–Nashville, Texas Triangle, etc.)

## 🗺️ Figures

![Map](AHR%20V2%20Fig%201.png)
![Failure Nodes](AHR%20%V2%20Fig%202.png)
![Baseline Performance](AHR%20V2%20Fig%203.png)
![Monte Carlo Distribution](AHR%20V2%20Fig%204.png)
![Most important connectors](AHR%20V2%20Fig%205.png)

---

# Urban Traffic Flow & Resilience Model (Huntsville Case Study)

## Overview
This project develops a network-based traffic simulation model to analyze congestion propagation, system resilience, and infrastructure vulnerability in Huntsville, Alabama.

The model evaluates how disruptions, demand variability, and time-of-day patterns impact system performance, with a focus on identifying critical bottlenecks and effective mitigation strategies.

---

## Key Features

- Directed network model of urban traffic corridors
- Volume-delay congestion modeling (BPR function)
- Monte Carlo simulation for stochastic demand and incidents
- Time-of-day demand modeling (AM Peak, PM Peak, Midday, Night)
- Scenario analysis (baseline, incident, and targeted improvement)
- Visualization of network congestion and system performance

---

## Key Results

- Disruption of a critical corridor (I-565) increased total system delay by **+1851%**
- Monte Carlo simulation revealed a **low-frequency, high-impact failure system (~6% probability)**
- Targeted improvements to alternate corridors restored system performance to baseline levels
- AM Peak produced the highest congestion, indicating vulnerability due to concentrated inbound demand

---

## Methodology

- Graph-based traffic network (nodes = zones, edges = corridors)
- Shortest-path traffic assignment with iterative updates
- Nonlinear congestion modeled using volume-delay functions
- Stochastic simulation with random incidents and demand variability

---

## Visualizations

### Baseline Network
![Baseline](HSV_Traffic_Map_Fig.%201.png)

### Incident Scenario
![Incident](HSV_Traffic_Map_Incident_Fig.%202.png)

### Monte Carlo Delay Distribution
![Monte Carlo](HSV_MC_Distribution_of_Delay_Fig_4.png)

### Time-of-Day Analysis
![Time of Day](HSV_Time_of_Day_Delay_Fig%205.png)

---

## Tools & Technologies

- Python
- NumPy, Pandas
- NetworkX
- Matplotlib
- Monte Carlo Simulation

---

## Report

Full analysis available here:

[Traffic Flow & Resilience Report](HSV%20Traffic%20Model%20Report.pdf)


# Reinforcement Learning for JIT Manufacturing Optimization (RL -vs- Reactive)
A reinforcement learning-based decision system that reduces shortages and overtime in JIT manufacturing, improving both reliability and cost efficiency under uncertainty.

### Impact:
- ↓ Shortages by ~17%
- ↓ Overtime by ~19%
- ~$2,280 annual cost savings
  
## Overview

This project develops a reinforcement learning (RL)-based decision support system for a simulated Just-in-Time (JIT) manufacturing environment under stochastic disruptions.

The goal is to improve operational decision-making by reducing:
- Production shortages
- Unnecessary overtime
- Overall system cost

A Q-learning agent is trained to replace a traditional threshold-based reactive policy.

---

## Problem Context

JIT manufacturing systems minimize inventory but are highly sensitive to disruptions. Traditional control policies rely on fixed inventory thresholds, which are reactive and do not account for uncertainty or system dynamics.

This project explores whether RL can provide a more adaptive and efficient control strategy.

---

## Methodology

- Simulation of a dual-shift manufacturing system
- Stochastic demand and supply disruptions
- Q-learning reinforcement learning agent
- 500 training episodes
- 50 independent evaluation runs (Monte Carlo simulation)

### Actions:
- 0 → Do nothing
- 1 → Call overtime

#Results

![Reward comparison](RL%20vs%20Reactive%20Fig.%201.png)

![Shortage comparison](RL%20v%20Reactive%20Figure%202.png)

![OT comparison](RL%20vs%20Reactive%20Fig.%203.png)

![Cost comparison](Rl%20vs%20Reactive%20Cost%20Comparison.png)


## Key Insight

Unlike traditional threshold-based policies, the RL agent learns system context (inventory levels and disruption states) and selectively applies overtime only when it is truly beneficial.

This results in a dominant decision strategy—simultaneously improving shortage reduction and cost efficiency without the typical tradeoff between reliability and operational cost.

## Tech Stack

- Python
- NumPy
- Matplotlib
- Reinforcement Learning (Q-Learning)
- Jupyter / Google Colab


## Full Report

[View Full Project Report](RL%20v%20Reactive%20Report.pdf)



### TVA Grid Cascading Failure Simulation
Network model of the Tennessee Valley Authority power grid analyzing cascading failure propagation and systemic blackout risk.

Tech used:
Python, NetworkX, Monte Carlo simulation, Matplotlib

Key outcomes:
• Identified critical grid nodes that amplify cascading failures  
• Modeled blackout probability across transmission corridors

---
### Cascade Participation Heatmap
![TVA Grid Heatmap](TVA%20Grid%20Heatmap.png)

---
### Transmission Network Map
![TVA Grid Map](TVA%20Grid%20Map.png)

---
### Blackout Probability Map
![TVA Blackout Probability Map](TVA%20Blackout%20Probability%20Map.png)

---
### Critical Trigger Locations
![TVA Critical Blackout Trigger Map](TVA%20Critical%20Blackout%20Trigger%20Map.png)

## Full Report

[View Full Project Report](TVA%20Cascade%20Report.pdf).

---
### Predictive Parts Shortage Risk Modeling in JIT Manufacturing
Machine learning model predicting parts shortages in a just-in-time production system with closed-loop operational decision control.

Tech used:
Python, Scikit-learn, Random Forest, Monte Carlo simulation

Key outcomes:
• Reduced simulated shortage occurrence  
• Evaluated operational tradeoffs between overtime and inventory stability

---
**Inventory Trajectory with Closed Loop**
![Figure 1](Figure%201.png)

---
**Inventory Trajectory Human vs ML**
![Figure 2](Figure%202.png)

---
**Distribution of OT over Simulations**
![Figure 3](Figure%203.png)

---
**Distribution of Shortage Risk Reduction (Human vs ML Policy)**
![Figure 4](Figure%204.png)

## Full Report

[View Full Project Report](ISE%20726%20Final%20Project.pdf)

---

### Weather-Driven JIT Supply Chain Disruption Model
Simulation of how regional weather events propagate through supplier networks to impact manufacturing production schedules.

Tech used:
Python, stochastic simulation, inventory modeling

Key outcomes:
• Modeled supply disruption risk  
• Evaluated production resilience strategies

---
**Weather Figure Loss Distribution**
![JIT_Weather_Figure_Loss_Distribution](JIT_Weather_Figure_Loss_Distribution.png)

---
**Weather Corridor Vulnerability**
![JIT_Weather_Vulnerability_Radar](JIT_Weather_Vulnerability_Radar.png)

---
**Severe Weather Supply Chain Survivability Curve**
![JIT_Weather_Survival_Curve](JIT_Weather_Survival_Curve.png)

---
**Inventory Buffer Heatmap**
![JIT_Weather_Heatmap](JIT_Weather_Heatmap.png)

## Full Report

[View Full Project Report](JIT%20Weather%20Report.pdf)

---


## Technical Skills

Languages
Python, SQL

Libraries / Tools
NetworkX, NumPy, Pandas, Scikit-learn, Matplotlib

Methods
Monte Carlo simulation
Machine learning
Systems modeling
Network analysis

I also have certification in FANUC Robotics during my time as a robot doctor at Mazda Toyota Manufacturing, as well as hands-on experience with the robots, including building applicators, helping install lines, as well as work with PELT machines for paint film builds, wave scan meters, and color meters. 

## Contact

I’m actively seeking opportunities in systems engineering, manufacturing engineering, or data-driven operations roles. My phone number is (256)627-7162 and my email is gilmer72086@yahoo.com
