
https://github.com/user-attachments/assets/486ef54b-33f1-46f8-ab11-f61b35857d6f
# **Proximal Policy Optimization (PPO)**

### **Overview**

This repository contains a from-scratch implementation of Proximal Policy Optimization (PPO) in PyTorch, tested on the challenging Ant-v5 environment from Gymnasium.

PPO is one of the most popular on-policy reinforcement learning algorithms — striking a balance between stability and performance. Unlike vanilla policy gradients that can collapse due to large updates, PPO introduces a clipped surrogate objective that ensures safe, controlled learning steps while still improving efficiency.

## **Why PPO is Powerful ?**

    🚦 Stable Training: Uses clipped updates to prevent policy from diverging.
    
    ⚡ Sample Efficiency: Reuses on-policy data effectively without the instability of TRPO.
    
    🧠 General-Purpose: Performs well across continuous control (Ant, Humanoid, Walker2d) and discrete domains (Atari).
    
    🏋️ Proven Scalability: Deployed in robotics, game-playing, and simulated control tasks at scale.

### **Results**

This implementation has been successfully tested on Ant-v5, where the agent learns to walk and survive in a complex continuous-control environment.

📹 Example training video (Ant-v5): Uploading Untitled video - Made with Clipchamp (7).mp4…

#### **Performance milestone:**

✅ Ant-v5 agent reached 812 episodic reward at episode 155 from scratch.

### **Core Idea Behind PPO**

At its heart, PPO tries to maximize the expected reward while keeping new policies close to the old ones.

This means updates never push the new policy too far away from the old one, making learning both fast and safe.

## **Use Cases**

PPO is widely used across domains where continuous and discrete action control is required:

    🤖 Robotics: Training robots to walk, grasp, and manipulate objects.
    
    🎮 Games: Agents mastering environments like Atari, MuJoCo, and Unity.
    
    🌍 Simulation & Research: Benchmarking RL algorithms on control tasks.
    
    🚀 Real-World Applications: Self-driving policies, recommendation systems, and adaptive decision-making.

### **Repository Structure**

    ppo_ant.ipynb → Jupyter Notebook with PPO implementation tested on Ant-v5.
    
    plot.py → Script for visualizing training curves (losses, rewards).
    
    videos/ → Training rollout videos for inspection & sharing.

#### **License**

This project is licensed under the MIT License.
