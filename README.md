# 🚦 Traffic Lights Metering System with Reinforcement Learning

This project presents a reinforcement learning–based system for optimizing highway **ramp metering** using both **Q-learning** and **Deep Q-Networks (DQN)**. The agent learns optimal traffic light control policies through interaction with a SUMO simulation environment, improving traffic flow while minimizing congestion and queue buildup at the ramp.

---

## 📌 Objectives

- Simulate a realistic highway–ramp network using **SUMO**
- Train RL agents to **dynamically control traffic lights**
- Reduce **ramp queue lengths** and **improve highway flow**
- Explore **reward function design** and **hyperparameter tuning**
- Compare **Q-learning** and **DQN** performance

---

## 🧠 Reinforcement Learning Overview

- **Q-learning**: Off-policy tabular method with state-action value updates
- **DQN**: Deep neural network approximation with:
  - Experience Replay
  - Target Networks
  - Epsilon-Greedy exploration

### 🔁 State Representation
Each state is defined by:
- **Highway traffic density** (normalized)
- **Ramp queue length** (normalized)
- **Traffic light phase** (discrete: green, yellow, red)

### 🎯 Action Space
- Action 0: Green Light (Ramp flow allowed)
- Action 1: Yellow Light (transition phase)
- Action 2: Red Light (Ramp flow stopped)

### 🧮 Reward Function
Weighted combinations of:
- **Highway flow**
- **Average speed**
- **Ramp queue penalty**

Dynamic reward strategies were tested and tuned across multiple experiments.

---

## 🛠️ Technologies & Tools

| Component      | Tool/Library           |
|----------------|------------------------|
| Simulation     | [SUMO](https://www.eclipse.org/sumo/) + TraCI |
| RL Algorithms  | Python, NumPy, TensorFlow, Keras |
| Visualization  | Matplotlib             |
| Scripts & Logs | XML, CSV, Python       |

---

📄 report.pdf      ← Technical report (Full documentation)

