# Squid Game – Unreal Engine 5.6

<p align="center"> <img src="https://via.placeholder.com/800x400.png?text=Squid+Game+UE5+Project" alt="Game Thumbnail" width="100%"> </p>

![Unreal Engine](https://img.shields.io/badge/Engine-Unreal_5.6-black?style=for-the-badge&logo=unrealengine)
![Language](https://img.shields.io/badge/Language-C%2B%2B_%26_Blueprints-blue?style=for-the-badge&logo=cplusplus)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows)
![Status](https://img.shields.io/badge/Status-Prototype-orange?style=for-the-badge)

📖 Project Overview

A mini-game inspired by the Squid Game series, developed using Unreal Engine 5.6.
The project focuses on implementing survival-based rounds with strict rule systems, trigger-based events, and elimination mechanics using a hybrid C++ and Blueprint architecture.

This project is created for learning, hackathons, and portfolio demonstration.

🎮 Available Game Rounds

🟢🔴 Red Light, Green Light

Player can move only during Green Light.

Any movement during Red Light results in elimination.

AI detection + movement checks are used for rule enforcement.

🪢 Jump Rope

A rotating rope moves with physics-based collision.

Player must time jumps to survive.

Collision with rope leads to instant elimination.

---

🧰 Tech Stack & Tools

🎮 Engine: Unreal Engine 5.6

💻 Programming: C++ and Blueprints

🎨 Modeling: Blender

🧍 Animations: Mixamo

🛒 Assets: FAB and Sketchfab (licensed)

⚙️ Systems Used:

- Trigger Volumes
- Physics Simulation
- AI Perception
- Custom Game Modes and Managers

---

## 📂 Project Structure

The project maintains a professional modular structure for scalability:

```text
Content/
 ├── Blueprints/                           # Core gameplay logic, triggers, managers
 ├── CR/                                   # Custom round systems and round-specific assets
 ├── Characters/                           # Player character and NPCs
 ├── Image/                                # UI images and textures
 ├── LevelPrototyping/                     # Prototype levels (Red Light, Jump Rope)
 ├── Resources/                            # Materials, sounds, and common assets
 ├── Sci-Fi_Shots_Pack2_Game_Of_Weapons/   # Third-party environment & weapon props
 ├── TPBDMat/                              # Material instances and shaders
 ├── ThirdPerson/                          # Default UE third-person framework assets
 ├── __ExternalActors__/                   # World Partition external actor data
 ├── __ExternalObjects__/ThirdPerson/Maps/ThirdPersonMap
 └── meyer_weapon_mountain_camo/           # Weapon asset pack
```

🗺️ Levels

All playable maps are located in:

Content/LevelPrototyping/

Available Maps

- RedLight_Level — Red Light, Green Light round
- JumpRope_Level — Jump Rope survival round

▶️ How to Run the Project
✅ Prerequisites

- Unreal Engine 5.6
- Visual Studio 2022 with C++ Game Development workload

⚙️ Setup Steps

1. Right-click the `.uproject` file
2. Click Generate Visual Studio project files
3. Open the generated `.sln` file
4. Build the solution in Visual Studio

▶️ Play

1. Open the project in Unreal Engine
2. Go to `Content/LevelPrototyping/`
3. Open any level
4. Click Play (▶)

🧪 Testing Checklist

Verified mechanics:

- Movement detection during Red Light works correctly
- Elimination triggers on rule violation
- Rope collision physics works as expected
- Finish trigger qualifies player successfully

🚀 Planned Features

- Glass Bridge Round
- Honeycomb (Dalgona) Challenge
- Tug of War Mode
- Main Menu with Round Selection
- Sound Effects and Voice Announcements
- Global Round Progression System
- Multiplayer Support

📌 Disclaimer

This project is made for educational and portfolio purposes only.

It is a fan-made project inspired by Squid Game.

No official copyrighted content is claimed.

All third-party assets from FAB, Sketchfab, and asset packs are used under their respective licenses.

🙌 Developer

Prajjawal Vaishya
Game Programmer | Unreal Engine | C++ | Blueprints

If you like this project, feel free to ⭐ the repository!
