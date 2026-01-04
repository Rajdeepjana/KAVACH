# KAVACH Train Control System
An Arduino-based train signal and locomotive control simulation inspired by Indian Railways’ KAVACH safety system.

## Motivation: 
Railway safety is critical in India. KAVACH (train collision avoidance system) prevents accidents by enforcing signals and speed control.
This simulation demonstrates signal-based speed regulation, emergency braking, and realistic acceleration/deceleration, highlighting the importance of automated safety systems.

## Features
- Trackside signal sender (Green, Yellow, Red)
- Locomotive receiver with LCD dashboard
- Physics engine simulating train acceleration/deceleration
- Speed enforcement based on signals
- Serial telemetry for debugging

## Folder Structure
├── Phase1_Trackside
├── Phase2_Locomotive
├── Phase3_Physics
├── Docs
└── README.md

## How to Run
1. Clone the repository
2. Open Arduino IDE
3. Upload Trackside code to sender board
4. Upload Locomotive code to receiver board

## Example Output
## LCD Display:
-SIGNAL: GREEN
SPD: 120

SIGNAL: YELLOW  (blinking)
SPD: 80 OVR

SIGNAL: RED !!!
SPD: 0 BRAKE

## Serial Monitor (Telemetry):
SIGNAL -> G
SPD_ACTUAL: 120 | SPD_TARGET: 120 | DRIVER_REQ: 120

SIGNAL -> Y
SPD_ACTUAL: 80 | SPD_TARGET: 80 | DRIVER_REQ: 120 | OVERRIDE

SIGNAL -> R
SPD_ACTUAL: 0 | SPD_TARGET: 0 | DRIVER_REQ: 50 | OVERRIDE


## Future Work
Obstacle detection and automatic emergency braking

Web-based monitoring dashboard

GPS/GSM integration for real-time train tracking

AI-based prediction for optimal train speed

## About
Developed by Rajdeep Jana








