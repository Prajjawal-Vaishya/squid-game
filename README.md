# 🦑 Squid Game Simulation (Unreal Engine)

![Project Banner](https://via.placeholder.com/1200x400?text=Squid+Game+Simulation+Project)
*(Note: Replace the link above with a screenshot of your actual game)*

## 📖 Project Abstract
This project is a high-fidelity 3D simulation of the "Squid Game" series, built to demonstrate advanced gameplay programming, state management, and physics interactions within **Unreal Engine**.

The goal was to move beyond simple visual replication and implement fair, competitive mechanics using C++ and Blueprint scripting.

## 🕹️ Playable Levels

### 1. Red Light, Green Light
The core survival mechanic involving precision movement and reaction time.
* **The Logic:** Instead of simple input checking, the game monitors the player character's **velocity vector**.
* **The Challenge:** Players must manage their momentum. Stopping input immediately does not guarantee safety if the character is still sliding due to physics friction.
* **Elimination:** Instant ragdoll physics simulation is triggered upon detection of movement during the "Red Light" state.

### 2. Rope Jump
A physics-based agility challenge requiring timing and rhythm.
* **The Logic:** Uses dynamic collision detection to simulate a swinging rope.
* **The Challenge:** The rope speed varies, requiring the player to visually estimate the swing arc and jump apex.
* **Implementation:** Utilizes precise collision primitives to ensure hit detection is pixel-perfect and fair.

## 🛠️ Technical Implementation
This project showcases the following technical skills:

* **Core Engine:** Unreal Engine 5
* **Programming:** C++ (Core Logic) & Blueprints (UI/Animation Integration)
* **Physics:** Chaos Physics Engine (Ragdolls & Collision)
* **State Management:** Custom GameMode and PlayerController classes to handle round loops, elimination states, and win conditions.

### Key Code Highlight (Conceptual)
*Implemented a tolerance threshold for movement detection to account for network latency and micro-movements:*

```cpp
// Pseudocode logic used in the project
void AMyCharacter::CheckMovement()
{
    if (bIsRedLightActive)
    {
        float CurrentSpeed = GetVelocity().Size();
        if (CurrentSpeed > MovementTolerance)
        {
            EliminatePlayer();
        }
    }
} 

## 🎮 Controls

| Input | Action |
| :--- | :--- |
| **W, A, S, D** | Movement Control |
| **Space Bar** | Jump (Crucial for Level 2) |
| **Mouse Look** | Camera Control |
