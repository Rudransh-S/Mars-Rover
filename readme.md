# Mars Rover

This project involves the design and development of a Mars Rover prototype from the ground up. The primary objective is to replicate the fundamental capabilities of NASA-style rovers. The rover is being built to demonstrate essential planetary exploration functions such as all-terrain mobility, real-time obstacle avoidance, wireless/manual control, and potential for semi-autonomous behavior using onboard sensors.

# Building Procress

## Conceptualization & CAD Design
We began by exploring existing Mars rover mechanisms, especially NASA’s open-source JPL Rover Mechanical Design library. This resource helped us understand the fundamentals of the rocker-bogie suspension and its advantages on rough terrains.
- **Reference Material**: NASA JPL GitHub library

- **Customizations**: While inspired by JPL designs, we introduced our own modifications to the CAD based on material availability and simplicity of assembly.

**Tools Used**: Fusion 360 was our primary design software, enabling precise simulations and iterative design updates.

## Fabrication and Mechanical Assembly
Once the design was finalized:

- Parts were cut using waterjet and laser cutting tools, focusing on accuracy.

- During the first assembly, we encountered issues with misalignments and tolerance mismatches. This led us to revise several components and re-fabricate some joints.

- Critical Milestone: Assembling the rocker-bogie mechanism was one of the most crucial stages.

![alt text](</assets/image.png>)

![alt text](</assets/photo 2.jpeg>)
## Initial Electronic
Before diving into full sensor integration or semi-autonomous systems, we carried out basic electronic testing to validate the mechanical integrity and test power delivery to the motors.

We used a minimal setup for this stage:

Motor Control: Three L298N dual H-bridge motor drivers, each controlling two motors (one driver per wheel pair).

Power Supply: All three drivers were connected to a common regulated 12 volt power supply.

Microcontroller: An ESP32 DevKit was used to control the motors via Bluetooth using the Remote XY app.

Control Strategy: Pulse Width Modulation (PWM) was used to modulate speed, with directional control managed through the H-bridges.

Initially, the system performed as expected — the rover could move forward and backward on command.

However, unexpectedly, the setup stopped functioning reliably. Despite replacing individual components (motor drivers, ESP32, power connectors), the issue persisted.

This failure prompted a complete redesign of the electronics subsystem.

During the testing phase of our Mars Rover prototype, we encountered a critical mechanical limitation in the linkage between the servo motor and the steering wheel assembly. Specifically, the connection interface we had initially designed was not robust enough to withstand the operational loads, especially when the rover was tested on even surfaces. This failure compromised steering control, leading to unresponsiveness during maneuvering tests.




