# SyncGrid: The Decentralized Physics-Informed Smart Grid

## 🌍 Vision & Core Concept
SyncGrid is a next-generation decentralized control system designed to transform traditional power grids into resilient, self-optimizing microgrids. By integrating **Real-time Physics** with **Reinforcement Learning**, SyncGrid empowers prosumers to balance the grid locally while maintaining economic sovereignty.

## 🛠 Strategic Innovations

### 1. Physics-Informed Sensitivity (The Active Pulse)
Unlike traditional systems, SyncGrid utilizes a proprietary **Active Micro-Injection** technique. The firmware performs surgical injections of reactive power ($\Delta Q_{inv}$) to decouple physical variables ($\partial V / \partial Q$ and $\partial V / \partial P$), ensuring absolute measurement accuracy even in noisy environments.

### 2. The AI Architecture: Spatio-Temporal Awareness
The "Brain" of SyncGrid is built on a **Physics-Informed Graph Attention Network (GAT)**. It utilizes power-flow sensitivities to embed spatial awareness directly into the agent's perception. On the server side, a **KAN-FACMAC Mixer** coordinates thousands of agents while ensuring total explainability of global decisions.

### 3. Hardware-Aware Sim-to-Real Environment
To bridge the gap between simulation and reality, SyncGrid features a **Clipper Emulator**. This safety layer ensures that AI decisions never exceed the physical limits of the battery or inverter hardware.

### 4. High-Performance Data Pipeline
Engineered for scale, the system leverages a modern data stack including **Ray, Polars, and GreptimeDB** to process IoT streams with sub-millisecond latency.

## 📂 Repository Structure & Layers

SyncGrid is organized into four distinct architectural layers, each representing a critical component of the decentralized ecosystem:

1. **[Firmware/](./firmware):** The Physics-Informed Sensitivity module. Handles real-time $\Delta Q$ injections and hardware-level signal processing.
2. **[Infrastructure/](./infrastructure):** The Data Pipeline. Manages the modern data stack (Ray, Polars, GreptimeDB) and IoT ingestion core.
3. **[Environment/](./environment):** The Simulation Gym. Contains the `Clipper Emulator` and the `PowerGAT_MDN` surrogate physics engine for safe training.
4. **[Agent/](./agent):** The Decentralized Brain. Houses the SAC agent, Graph Attention Networks (GAT), and the explainable KAN-FACMAC mixer.

## ⚖️ Anti-Monopoly & Licensing
This project is licensed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**. 
- **Freedom to Innovate:** Anyone is free to use, study, and modify this system.
- **Anti-Lock-in:** Any commercial entity utilizing this core logic in a network service MUST share their source code under the same license.
- **Prior Art:** This public documentation serves as legal proof of original invention to prevent restrictive patenting by third parties.

---
**Lead Architect:** Mudaser  
**Developed by:** AretCore Labs  

**Copyright (c) 2026 Mudaser (AretCore). All rights reserved.**
# Licensed under AGPL-3.0
