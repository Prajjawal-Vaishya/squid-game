# 🦑 Squid Game – Unreal Engine 5.6

![Unreal Engine](https://img.shields.io/badge/Engine-Unreal_5.6-black?style=for-the-badge&logo=unrealengine)
![Language](https://img.shields.io/badge/Language-C%2B%2B_%26_Blueprints-blue?style=for-the-badge&logo=cplusplus)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows)
![Status](https://img.shields.io/badge/Status-Prototype-orange?style=for-the-badge)

A high-fidelity survival mini-game inspired by the *Squid Game* series, developed using **Unreal Engine 5.6**. This project leverages a hybrid architecture of **C++ for core logic** (movement detection, elimination states) and **Blueprints for gameplay flow**.

## 🎮 Game Modes

### 1. 🟢🔴 Red Light, Green Light
The classic survival game focusing on precision movement.
* **Rules:** Move only when the light is Green. Any movement detected during Red Light results in immediate elimination.
* **Core Mechanics:** * `C++` Movement Velocity Detection (Zero-tolerance logic).
    * Global Light State Manager (Syncs Audio, Visuals, and Kill Logic).
    * Finish Line Trigger Zones.

### 2. 🪢 Jump Rope
A timing-based endurance round.
* **Rules:** Jump over the rotating rope to survive. Touching the rope triggers the Ragdoll physics state.
* **Core Mechanics:**
    * Procedural Rotation logic for the rope.
    * Precise Collision Detection bubbles.
    * End-level qualification platform.

---

## 🛠️ Tech Stack & Implementation

| Component | Technology Used | Description |
| :--- | :--- | :--- |
| **Game Engine** | **Unreal Engine 5.6** | Utilizing Nanite & Lumen for visuals. |
| **Core Logic** | **C++** | Used for Movement Component & Game States. |
| **Scripting** | **Blueprints** | Visual scripting for UI and Animation graphs. |
| **3D Assets** | **Blender** | Custom props, environment block-outs. |
| **Animation** | **Mixamo** | Character rigging and locomotion. |
| **Physics** | **Chaos Physics** | Ragdoll simulation upon elimination. |

---

## 📂 Project Structure

The project maintains a professional modular structure for scalability:

```text
Content/
 ├── Blueprints/                 # Game logic, triggers, managers (BP_GameMode, etc.)
 ├── CR/                         # Custom Round-specific assets
 ├── Characters/                 # Player and NPC blueprints + skeletons
 ├── Image/                      # UI assets (Widgets, HUD textures)
 ├── LevelPrototyping/           # Main Maps (RedLight_Map, JumpRope_Map)
 ├── Resources/                  # Shared Materials and Sound Cues
 ├── Sci-Fi_Shots_Pack2/         # Environment modules
 ├── Weapons/                    # GrenadeLauncher (Experimental mechanics)
 └── C++ Classes/                # Custom Movement & GameInstance classes
