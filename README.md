# Capstone Project: Line Follower Robot (with Obstacle Detection)

An autonomous robot that follows a black line on a contrasting surface using IR sensors and Arduino, with added obstacle detection using an ultrasonic sensor.

## 🧠 Introduction

A **Line Following Robot** is an autonomous device designed to follow a specific path (usually a black line on a white surface or vice versa) using optical sensors. The robot uses arrays of IR sensors to detect the line and DC gear motors for movement, controlled by an **Arduino Uno**. An **ultrasonic sensor** is integrated for obstacle detection, enabling the robot to stop and avoid collisions automatically.

This project demonstrates core concepts in robotics, sensor integration, and motor control, and has practical applications in industrial automation, entertainment, and navigation systems.

## 🚀 Features

- **Autonomous Navigation**: Follows a black line on a contrasting background using IR sensors.
- **Obstacle Avoidance**: Detects and stops for obstacles using an ultrasonic sensor.
- **Flexible Movement**: Capable of making precise turns and adjustments.
- **Environmentally Robust**: Insensitive to ambient lighting and noise.
- **Modular Design**: Easily expandable for future enhancements (e.g., color detection, LCD display, maze solving).

## 🔩 Components

| Component                   | Description                              |
|----------------------------|------------------------------------------|
| Arduino Uno                | Microcontroller for logic and control    |
| IR Sensors (Array)         | Detects line and provides feedback       |
| Ultrasonic Sensor (HC-SR04)| Detects obstacles in the robot’s path    |
| L298N Motor Driver         | Controls speed and direction of motors   |
| DC Gear Motors             | Drives the robot’s wheels                |
| Chassis                    | Physical frame for mounting components   |
| Wheels, Castor Wheel       | Provides mobility and stability          |
| Battery Holder & Batteries | Power supply for the system              |
| Breadboard & Jumper Wires | Circuit connections                      |

## ⚙️ Working Principle

1. **Obstacle Detection**: The ultrasonic sensor continuously checks for obstacles. If detected, the robot stops.
2. **Line Detection**: Two IR sensors detect the black line.
   - If both sensors are on a white surface → robot moves forward.
   - If left sensor detects the line → robot turns left.
   - If right sensor detects the line → robot turns right.
   - If both sensors lose the line → robot stops.
3. **Motor Control**: The Arduino processes sensor inputs and commands the L298N motor driver to control the motors.

## 🔧 Circuit Diagram & Assembly

### Basic Connections

[IR Sensor 1] -----------> [Arduino]
[IR Sensor 2] -----------> [Arduino]
[Ultrasonic Sensor] -----> [Arduino]
[Arduino] ---------------> [L298N Motor Driver] ---> [DC Motors]
[Battery Holder] --------> [Arduino & Motor Driver]


### Assembly Steps

- Mount IR sensors at the front of the chassis, facing downward.
- Position the ultrasonic sensor in front for obstacle detection.
- Attach DC motors to the chassis and connect to the motor driver.
- Wire components to Arduino and motor driver.
- Connect battery holder for power supply.

## 🧪 How to Use

1. **Assemble the Robot**: Mount and wire all components as shown above.
2. **Upload Code**: Use the Arduino IDE to flash the provided code.
3. **Calibrate Sensors**: Adjust IR sensor sensitivity using potentiometers.
4. **Test the Robot**: Place it on a track and observe its movement.
5. **Obstacle Testing**: Place an obstacle to verify stopping behavior.

## 🏭 Areas of Application

- **Industrial Automation**: Material carriers in factories.
- **Entertainment**: Robot toys, educational kits.
- **Navigation**: Museum tour guides, exhibition bots.

## 🌱 Future Scope

- Maze solving algorithms
- Color detection sensors
- Path learning AI integration

## 🎓 Lessons Learned

- **Hardware Integration**: Hands-on circuit building.
- **Sensor Calibration**: Importance of tuning for accuracy.
- **Problem Solving**: Debugging both hardware and software.
- **Teamwork**: Collaborative engineering and testing.

## 🔮 Future Enhancements

- **Color Sensor**: Respond to different colored lines.
- **LCD Display**: Display real-time data (e.g., distance).
- **CCD Camera**: Advanced path detection and navigation.
- **Servo Motors**: For intelligent obstacle avoidance.

## 👨‍💻 Team Members

| Name                          | Roll No       |
|-------------------------------|---------------|
| Borru Vijay Sai               | 22EC01036     |
| Kakaraparthy Mohith Prakash   | 22EC01002     |
| Kotikalapudi Rohith V S D M   | 22EC01010     |
| Yedupati Harsha Vardhan       | 22EC01007     |
| C V Harshith Reddy            | 22CS01013     |

## 🤝 Contributing

Feel free to **fork this project**, **report issues**, or **submit pull requests** to improve or extend functionality!
