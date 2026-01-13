# 🦑 Squid Game Simulation: Unreal Engine Implementation

![Project Banner](https://via.placeholder.com/1200x400?text=Squid+Game+Simulation+Project)
*(Replace the link above with a screenshot or banner of your actual gameplay)*

## 📖 Project Overview
This project is a high-fidelity 3D survival simulation developed using **Unreal Engine**. It recreates the high-stakes atmosphere of *Squid Game* with a focus on realistic physics, precise movement mechanics, and custom C++ logic.

Unlike simple visual recreations, this project focuses on **state management** and **physics-based gameplay interactions** to create a fair but challenging competitive environment.

## 🔗 Project Links

| Platform | Link |
| :--- | :--- |
| **itch.io (Playable Build)** | **[Click Here to Play / Download](YOUR_ITCH_IO_LINK_HERE)** |
| **GitHub (Source Code)** | [View Repository](YOUR_GITHUB_LINK_HERE) |
| **Video Demo** | [Watch on YouTube](YOUR_YOUTUBE_LINK_HERE) |

## 🎮 Playable Levels

### 1. Red Light, Green Light 🔴🟢
The classic survival mechanic where precision is critical.
* **The Logic:** The game uses a custom GameState to control the "Doll" timer and rotation.
* **Movement Detection:** Instead of relying solely on input presses, the logic monitors the character's **velocity vector**. If the character retains momentum (sliding) after the "Red Light" triggers, they are eliminated.
* **Death Mechanic:** Triggers a Chaos Physics ragdoll simulation instantly upon elimination.

### 2. The Rope Jump 🪢
A custom agility level designed to test player timing and depth perception.
* **The Logic:** Features a physics-driven rotating obstacle (rope) with variable speed.
* **The Challenge:** Players must time their **Jump** action perfectly to clear the rope's hitbox.
* **Implementation:** Utilizes precise collision primitives (Capsule/Box components) to ensure hit detection is accurate and responsive.

## 🛠️ Technical Implementation
This project serves as a technical showcase for:
* **Engine:** Unreal Engine 5
* **Core Logic:** Hybrid implementation using **C++** for performance-critical logic (movement, state checks) and **Blueprints** for UI and animation handling.
* **Physics:** Chaos Physics Engine for ragdolls and collision handling.
* **Animation:** State Machines (AnimBP) blended with physics interactions.

## 🎮 Controls

| Input | Action |
| :--- | :--- |
| **W, A, S, D** | Movement Control |
| **Space Bar** | Jump (Crucial for Level 2) |
| **Mouse Look** | Camera Control |

## 🚀 Installation & Setup
To run this project locally (if not using the itch.io build):

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/Prajjawal-Vaishya/squid-game/
    ```
2.  **Generate Project Files:**
    * Navigate to the project folder.
    * Right-click the `.uproject` file.
    * Select **"Generate Visual Studio project files"**.
3.  **Build:**
    * Open the solution (`.sln`) file in Visual Studio.
    * Build for **Development Editor**.
4.  **Run:**
    * Launch the project in Unreal Engine.
    * Press **Play** in the editor.

## 🔮 Future Roadmap
* **Multiplayer Replication:** Implementing server-authoritative movement for competitive multiplayer.
* **Level 3 Expansion:** Adding the "Glass Bridge" level using Destructible Meshes.
* **AI Competitors:** Adding NPC bots with randomized reaction times to race against the player.

---
*Developed with Unreal Engine*
