# Kavach Train System

**Arduino-based Indian Railways Train Signaling & Locomotive Simulation**

This project simulates a train signaling system with:
- Trackside signals (Green, Yellow, Red)
- Locomotive dashboard with LCD displaying signal and speed
- Physics engine simulating acceleration/deceleration
- Yellow warning blink and speed limits (Indian freight train realistic)
- Modular phase-wise development (Phase 1 → Phase 5)

## Features
- Real-time train control using Arduino
- Robust serial communication between trackside and locomotive
- Physics-based train motion
- LCD dashboard with override indicators
- Expandable to obstacle detection and emergency braking modules

## Repository Structure
Kavach_Train_System/
│
├─ README.md
├─ LICENSE        (MIT or Apache 2.0, shows open-source professionalism)
├─ .gitignore     (ignore .vscode, .ino backups)
│
├─ Phase1_Trackside/   (sender arduino code)
│    └─ trackside_v1.ino
│
├─ Phase2_Locomotive/  (receiver dashboard)
│    └─ locomotive_v1.ino
│
├─ Phase3_Physics/     (inertia engine, acceleration simulation)
│    └─ locomotive_physics.ino
│
├─ Phase4_LCD/         (dashboard display and warnings)
│    └─ locomotive_lcd.ino
│
├─ Phase5_Final/       (all combined phases 1-5)
│    └─ locomotive_final.ino
│
├─ Docs/               (pictures, block diagrams, TinkerCAD screenshots)
│    └─ Kavach_BlockDiagram.png
│    └─ Simulation_Screenshot.png
│
└─ Notes/              (your design thoughts or phase notes)
     └─ Phase1-5_Notes.md

