Arena Navigation Robot
CoppeliaSim simulation of an autonomous arena navigation system — two robots working together to handle a sequence of tasks across multiple stations.

What it is
The idea was to simulate a robotic system that navigates an arena and handles a sequence of gate-triggered operations — pump activation, weight check, indicator display — mimicking how robots work in industrial automation environments.
Went full simulation in CoppeliaSim since building the complete hardware setup wasn't feasible in the timeframe. A custom UI handled the inputs that physical sensors would've provided in a real build.

System design
Two robots working together:
Robotic Arm (4-DOF)

Adapted from previous mobile manipulator work (Botivine)
Handles picking and placing at each station
320mm reach

Line-Following Robot

Autonomous navigation between stations
Proportional steering control
Obstacle detection

Station sequence:
Pump activation → LED indicator → Weight check → Display result

Simulation
Built entirely in CoppeliaSim. The custom UI replaces physical sensor inputs — each button press triggers the same logic that a real sensor would in hardware.

What I took from this
Simulation-first forces you to think through every state, every sensor input, every edge case before touching hardware. That process made the design much cleaner than jumping straight to building. Also got properly comfortable with CoppeliaSim's scripting environment.

Built at VFSTR September· 2025
