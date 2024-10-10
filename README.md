# Dorm Automation System

This is a 3-part program designed to automate control over physical objects and electronics in a dorm room using a Raspberry Pi Pico, a PythonAnywhere server, and a GitPages frontend.

## Components

### 1. **Pi Pico (Hardware Controller)**
   - Controls physical objects and electrical devices in the dorm, such as lights, fans, and other appliances.
   - Uses sensors, relays, servos, and more to automate the environment.
   - Communicates with the server hosted on PythonAnywhere to receive control signals and send data like sensor readings.

### 2. **Server (Hosted on PythonAnywhere)**
   - Acts as the central hub for communication between the Pi Pico and the frontend.
   - Stores settings, current states, and sensor data in a database.
   - Allows the Pi Pico and frontend to interact through API requests.
   - Handles logic to ensure efficient communication and synchronization between the hardware and the control interface.

### 3. **Frontend (Hosted on GitPages)**
   - Provides a user-friendly interface for controlling the dorm's lights, temperature, and other settings.
   - Logs dorm events such as door usage, temperature changes, and electrical usage.
   - Sends commands to the server, which then communicates with the Pi Pico to execute the necessary actions.

## Features
- **Automation**: Pi Pico automatically manages physical controls and monitors the dorm environment.
- **Centralized Control**: All settings and data are centralized and managed through the PythonAnywhere server.
- **Real-Time Interface**: The frontend hosted on GitPages allows real-time adjustments to the dorm setup.
- **Data Logging**: Track events and sensor data such as door activity, temperature readings, and usage statistics.

## How It Works
1. The **Pi Pico** receives data from sensors and sends it to the server, while also controlling electrical components.
2. The **Server** stores data and allows both the Pi Pico and the frontend to communicate seamlessly.
3. The **Frontend** provides controls for lights, appliances, and displays logged data from the dorm events.

## Requirements
- Raspberry Pi Pico
- PythonAnywhere account for hosting the server
- GitPages account for hosting the frontend
