# CLOSED-LOOP MOTOR CONTROL SYSTEM
Currently developing a closed-loop motor control system using an ESP32, 3-6V DC motor, L293D, 10k ohm potentiometer, and an obstacle avoidance module. It will be PID controlled.
- The project is coded with C++.
- Made a DIY tachometer using the obstacle avoidance module.
- The IR sensor in the obstacle avoidance module reads the the RPM of the motor speed when attaching a fan attachment.
- The DC motor PWM is controlled by the 10k ohm potentiometer.
## main components (these are the best components I have at the moment):
* ESP32 Microcontroller
* 3-6V DC Motor
* L293D Motor Driver
* Obstacle Avoidance Module (OAM)


## Current State
When the OAM is connected to the GPIO01 pin on the ESP32, false pulse readings are detected by the OAM even when the motor fan
isn't in front of the IR sensor. This could be due to electrical noise which means I could use decoupling capacitors to fix the
issue but for now I am not sure. I am currently trying to figure out why it happens.
