# 🚦 Smart Traffic Light Controller using Q-Learning

This project simulates a smart traffic light control system using **Reinforcement Learning (Q-Learning)**. The agent learns to optimize traffic flow at a simple intersection with two directions by minimizing congestion through intelligent traffic light switching.

## 📌 Features

- Simulates traffic movement at a 2-way intersection.
- Implements a Q-Learning agent to minimize vehicle queue lengths.
- Reward structure encourages smooth traffic flow.
- Simple and extensible Python implementation for educational use.

## 📁 Project Structure

traffic_rl/
- ├── traffic_controller.py # Core RL simulation code
- ├── README.md # This file


## 🚀 Getting Started

### Prerequisites

- Python 3.7+
- NumPy

### Installation

1. Clone the repository:
2. 
   git clone repository
   cd traffic_rl
   
Install dependencies:

pip install numpy
Run the simulation:

python traffic_controller.py
📊 How It Works
Environment: A basic traffic junction with cars arriving in two directions.

Agent: Chooses which direction gets the green light (A or B).

States: Number of cars waiting in each direction (0–5).

Actions: 0 for green light in direction A, 1 for green in B.

Reward: Negative sum of cars waiting (lower is better).

The agent improves over 1000 episodes, learning which actions lead to less congestion.

💡 Example Output

Episode 0, Total Reward: -380
Episode 100, Total Reward: -205
Episode 200, Total Reward: -190
...
Training complete. Sample Q-values:
State (0, 0), Action 0: Q-value = -0.02
State (0, 0), Action 1: Q-value = -0.01
...
📈 Future Enhancements
Upgrade to Deep Q-Network (DQN)

Integrate with real-time traffic data

Add visualization using Matplotlib or Pygame

Expand to multiple intersections (grid layout)

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
