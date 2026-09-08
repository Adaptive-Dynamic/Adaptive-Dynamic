# Adaptive-Dynamic
Senior Design Project - Speed-Adaptive Long-Range Proximity Warning System
## Executive Summary

Rear-end collisions can occur when drivers fail to recognize that a vehicle ahead is decelerating, particularly during extended highway driving where fatigue, distraction, or delayed reaction can increase stopping risk. Traditional proximity warning approaches may rely on fixed distance thresholds that do not adequately account for changes in vehicle speed and relative motion.

This project develops a **Speed-Adaptive Long-Range Proximity Warning System for Driver Assistance**. The system continuously monitors the host vehicle's speed, the relative motion of a leading vehicle, and the distance between the vehicles to determine whether the current following distance is safe.

### System Overview

The system will:

- Detect and track a leading vehicle using a long-range sensing technology.
- Measure the relative distance and speed between the host and leading vehicles.
- Acquire and process sensor data using an embedded controller.
- Calculate the required safe following and braking distance in real time.
- Compare the measured distance against the calculated safe distance.
- Provide an audible warning when an unsafe following condition is detected.

Several sensing technologies will be evaluated:

- **LiDAR**
- **Infrared Rangefinders**
- **Ultrasonic Sensors**
- **Camera-Based Computer Vision**

These technologies will be compared based on **range, accuracy, response time, cost, reliability, and implementation complexity** before selecting the most appropriate approach for the prototype.

### Engineering Scope

The project will integrate the selected sensing technology with embedded processing, sensor interfaces, analog signal-conditioning circuitry, power regulation, and the driver warning system.

A **speed-adaptive safe-distance algorithm** will continuously update the required braking distance based on the host vehicle's speed and relative motion with respect to the leading vehicle. When the measured following distance falls below the calculated safe distance, the system will activate an audible warning to notify the driver.

### Testing & Validation

The completed system will be evaluated using representative vehicle-following and deceleration scenarios. Testing will assess:

- Distance measurement accuracy
- Relative speed measurement accuracy
- Warning response latency
- Vehicle detection reliability
- Safe-distance calculation performance
- System stability
- Overall prototype functionality

Hardware and software will be iteratively refined based on testing results.

### Deliverables

The project will produce:

1. A fully operational proximity warning prototype
2. Integrated sensing and embedded-processing hardware
3. A real-time safe-distance calculation algorithm
4. An audible driver-warning system
5. Testing and validation results
6. A user guide
7. A maintenance manual

### Budget

The complete system will be developed within the available budget of **$240 per student**.
