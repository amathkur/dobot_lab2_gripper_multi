# Dobot Lab 2.2: Gripper Multi-Cube Manipulation (RAS545 - Arizona State University)

This repository contains code for **Lab 2.2 assignment** in the course **RAS545 (Robotics Automation Systems)** at **Arizona State University**.

## Overview

The provided Python script (`dobot_lab2_gripper_multi.py`) is designed to control the Dobot Magician robotic arm to **grab cubes using the gripper and place them in different locations**.

The script executes a sequence to pick up cubes from four locations and place them at four other locations, then reverses the operation to return the cubes to their original positions.

This assignment emphasizes using the **gripper end-effector** instead of suction.

## Features

- Controls the Dobot Magician via serial port (USB).
- Uses the gripper to pick and place up to 4 cubes.
- Hover height, waypoints, and motion parameters are customizable.
- Reduced speed and added rotation for precision at tricky pick/place spots.
- Both forward and reverse movement sequences are implemented.

## Usage

1. **Install dependencies**
   - Python 3.x
   - Dobot Python library (`pydobot` or `pydobot2`)

2. **Connect Dobot Magician** via USB.

3. **Run the script**:
   ```bash
   python3 dobot_lab2_gripper_multi.py --port /dev/ttyACM0 --hover 30 --v 200 --a 200
   ```

   - `--port` specifies the serial port (default: `/dev/ttyACM0`)
   - `--hover` specifies the hover height above each waypoint (default: 30 mm)
   - `--v` and `--a` specify linear speed and acceleration

4. **Customize waypoints** in the script for your specific lab setup if needed.

## Educational Purpose

This code is intended as a practical exercise for learning robotic manipulation and automation using the Dobot Magician with a gripper in the RAS545 course at ASU.

## License

This repository is for educational use in RAS545 at Arizona State University.
