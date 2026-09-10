# Task 2 – Communication Architecture

## Objective

The drone is primarily autonomous ,I assume, with the Pixhawk 6C Mini acting as the flight controller/autopilot. An RC link is retained for manual control and emergency override. Telemetry provides flight data to the ground station, while the VTX provides the live video feed.

## RC Transmitter & Receiver --> RadioMaster Pocket + ELRS RP1

## Reasons:

ELRS Protocol:
* Super Low Latency: ELRS provides a fast control link, allowing the drone to respond quickly to pilot inputs.

* Range: ELRS can provide a long-range control link, with the actual range depending on frequency, antenna setup, transmit power, interference and line of sight.

* Open Source: ELRS is free, constantly updated by a global community, and works with many brands.

* Frequency Hopping: ELRS constantly jumps between radio channels to dodge interference from Wi-Fi  or other pilots.

Radio Master Pocket 
* Hall Effect Gimbals: The sticks use magnets instead of rubbing parts, meaning they stay accurate and do not wear out.
* Compact Size: The Pocket is small, light, and has folding stick ends so it fits easily in a backpack.
* Built-In ELRS: It comes with ELRS ready to go, so you do not need to buy or plug in extra radio modules.
* EdgeTX Software: It runs a powerful operating system that lets you customize every switch, button, and voice alert.

## Telemetry Module --> Holybro SiK Telemetry Radio V3

## Reasons:

MAVLink Protocol:
* Bidirectional Communication: Allows the drone and ground station to exchange flight data and commands.

* Range: The 500mW version can provide around 1km line-of-sight range depending on antennas and interference.

* Reliable Data Link: Designed for sending flight information such as GPS position, altitude, battery status, and flight mode.

* Multiple Power Options: Available in different power versions, allowing a balance between range and power consumption.

Holybro SiK Telemetry Radio V3:
* Lightweight: The 100mW and 500mW versions weigh around 23.5g.

* UART Connection: Connects directly to the Pixhawk's telemetry UART port.

* Ground Station Support: The second radio can be connected to a laptop/ground station to receive the drone's telemetry.

* MAVLink Support: Compatible with the MAVLink protocol used by the Pixhawk.

## VTX --> Analog FPV Camera + Analog VTX

## Reasons:

Analog Video:
* Low Cost: Analog cameras and VTXs are significantly cheaper than most digital FPV systems.

* Low Latency: Analog video has very low latency, which allows the operator to see changes in the drone's view quickly.

* Lightweight: Analog cameras and VTXs can be very lightweight, helping keep the drone within its weight limit.

* Simple System: Analog video does not require a proprietary digital video ecosystem, making the system simple and widely compatible.

* Predictable Signal Loss: Analog video generally degrades gradually as the signal becomes weaker, producing increasing noise/static rather than suddenly freezing or cutting to a black screen.

Analog VTX:
* Transmits the camera's analog video signal wirelessly to the ground receiver.

* The VTX power and antenna determine the achievable range, which depends on the environment and interference.

* The ground station requires a compatible analog video receiver/goggles.

## Power Supply

* LiPo Battery: The main power source for the drone.

* Holybro PM02D Power Module: Connected between the LiPo battery and Pixhawk. It provides regulated power to the Pixhawk and allows battery voltage/current to be monitored.

* Pixhawk 6C Mini: Receives power from the power module.

* RC Receiver: Powered from the Pixhawk's regulated 5V supply.

* Telemetry Module: Powered from the Pixhawk's regulated 5V supply.

* VTX: Powered from the appropriate regulated power supply according to its required input voltage.


## Protocols and Ranges

* RC: ELRS 2.4 GHz → CRSF → Pixhawk UART. Provides a low-latency, long-range control link.

* Telemetry: MAVLink over UART → SiK wireless telemetry. Approximately 1km line-of-sight for the 500mW version with suitable antennas.

* VTX: 5.8 GHz analog video transmission. Range depends on VTX power, antenna, interference and line of sight.

