# 🦑 Squid Game: Advanced Physics Simulation

![Project Banner](https://via.placeholder.com/1200x400?text=Unreal+Engine+5+Simulation)

## 📖 Project Overview
This project is a technical demonstration of **High-Fidelity Survival Mechanics** built in **Unreal Engine 5**. The goal was to engineer a competitive simulation that relies on **C++ State Management** and **Chaos Physics** rather than simple scripted events.

Aligned with the principles of **Open Innovation**, this project "breaks the code" of standard platformers by implementing:
* **Vector-Based Movement Detection:** A custom algorithm that calculates player momentum vs. friction to determine elimination, rather than simple input checks.
* **Procedural Physics Interactions:** Utilizing the Chaos engine to create non-deterministic outcomes for ragdolls and destructible environments.

## 🔗 Project Links

| Platform | Link |
| :--- | :--- |
| **itch.io (Playable Build)** | **[Click Here to Play / Download](YOUR_ITCH_IO_LINK_HERE)** |
| **GitHub (Source Code)** | [View Repository](YOUR_GITHUB_LINK_HERE) |
| **Video Demo** | [Watch on YouTube](YOUR_YOUTUBE_LINK_HERE) |

## 🎮 Simulation Levels

### 1. The Velocity Protocol (Red Light, Green Light)
A test of precision and momentum management.
* **The Innovation:** The "Kill" logic is decoupled from user input. It monitors the `GetVelocity().Size()` of the Pawn. If physics friction fails to stop the character in time (simulating real-world inertia), the player is eliminated.
* **Tech Stack:** C++ Custom GameState, Chaos Ragdoll Physics.

### 2. The Apex Challenge (Rope Jump)
A study in dynamic collision and timing.
* **The Innovation:** Uses interpolating physics constraints to create a variable-speed hazard.
* **Tech Stack:** Dynamic Collision Primitives, Sine-Wave Interpolation.

## 🛠️ Technical Engineering
This project highlights advanced usage of Unreal Engine features:
* **Language:** C++ (Core Gameplay Logic) & Blueprints (Visual Scripting)
* **Physics Engine:** Chaos Physics (UE5)
* **Optimization:** Logic ticks are optimized for potential multiplayer replication.

## 🎮 Controls

| Input | Action |
| :--- | :--- |
| **W, A, S, D** | Movement Control |
| **Space Bar** | Jump (Crucial for Level 2) |
| **Mouse Look** | Camera Control |

## 🚀 Installation & Setup
1.  **Clone the Repository:**
    ```bash
    git clone [YOUR_GITHUB_LINK_HERE]
    ```
2.  **Generate Project Files:** Right-click `.uproject` > "Generate Visual Studio project files".
3.  **Build:** Open `.sln` in Visual Studio > Build for **Development Editor**.
4.  **Run:** Launch Unreal Engine > Press **Play**.

---
*Submitted for Review | Created with Unreal Engine 5*
