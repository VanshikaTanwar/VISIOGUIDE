# VISIOGUIDE
Cost-Efficient VisioGuide using VSDSquadron mini 
"Giving Mobility Vision to Blind and Deaf People"

# VISIOGUIDE__Product-Development

Cost-Efficient VisioGuide for Blind and deaf people using VSDSquadron mini 
***VISIOGUIDE, Powered by the VSDSquadron Mini***


TEAM VSD DIR-V-VISIOGUIDE


# Introduction to VISIOGUIDE

For those who are both blind and deaf, navigating the world can be extremely difficult. Current assistive technologies, like conventional white canes, frequently don't meet their specific needs and only offer a limited amount of information. The goal of this project is to use the VSDSQuadron Mini RISC-V board to create a "Cost-Efficient VisioGuide". This creative solution gives deaf-blind people more mobility, independence, and a sense of security in their daily lives by combining an ultrasonic sensor with a vibration motor to provide real-time obstacle detection and haptic feedback. This project aims to develop a truly impactful assistive technology that enhances the quality of life for this underprivileged community by utilizing the RISC-V platform's affordability, flexibility, and energy efficiency. 


# Overview of VISIOGUIDE

The goal of this project is to create a VisioGuide that is both affordable and easy to use for people who are blind and deaf. The system improves user safety and independence by integrating an ultrasonic sensor with the VSDSquadron Mini RISC-V board to provide real-time obstacle detection. With feedback patterns that can be altered to meet specific needs, the system uses haptic feedback to warn users of possible hazards. Because the RISC-V architecture is open-source, it can be expanded and customized in the future, guaranteeing that the solution will continue to be flexible enough to meet changing user needs. Additionally, the project maximizes battery life for extended use by utilizing the RISC-V core's energy efficiency. In addition to enhancing the lives of deaf-blind people, this solution shows how adaptable and affordable the VSDSquadron Mini is for creating cutting-edge assistive innovation.

This project's primary goal and Overview is to:

Deaf-blind people's mobility and independence should be greatly increased.

By using the VSDSQuadron Mini RISC-V board to create a smart blind stick, the project seeks to accomplish this. This gadget will have features such as:

Informative Haptic Feedback: To give important details about environmental barriers.
Reliable Obstacle Detection: To guarantee precise and prompt detection of possible dangers.
In order to provide deaf-blind people with the resources they require for safe and independent mobility, the project aims to improve safety, navigation, and general quality of life.


# Working of VISIOGUIDE System

1. Power Supply: The ESP32 module, DHT11, PIR, Touch sensors, relay module, and VSDSquadron Mini board all receive the required power from the 5V power supply. Appliances connected to the relay can have their AC mains power controlled by the AC Mains to Supply Power with Relay circuit. 

2. Acquisition of Sensor Data: -Temperature and humidity are measured by the DHT11 sensor. This information can be used to control appliances based on temperature (e.g., adjusting fan speed based on temperature). 
-Motion is detected by aaPIR sensor. Actions such as turning lights on when motion is detected and off after a predetermined amount of inactivity can be triggered by this. 
-Touch Sensor: Enables manual device control or the activation of particular actions through touch input.

3. Data Processing and Management: Data from the sensors (DHT11, PIR, Touch) is read by the VSDSquadron Mini. makes decisions by processing the sensor data (e.g., adjusting fan speed based on temperature, turning lights on/off based on PIR sensor input). It Transmits and receives commands by communicating with the ESP32 module. Data is received by the ESP32 Module from the VSDSquadron Mini. uses Wi-Fi to connect to the internet. sends information to the cloud (like the Arduino IoT Cloud) for remote access and storage. gets commands for control from the mobile app or the cloud. sends commands to the VSDSquadron Mini for control.

4. Appliance Control: The VSDSquadron Mini sends control signals to the relay module. Depending on the signals it receives, switches turn on and off the power to the connected appliances (lights, fans, etc.).

5. Control and User Interface: The Arduino IoT Remote mobile app allows users to communicate with the system. Track sensor data in real time (temperature, humidity). Remotely control appliances (fan speed, light on/off, etc.). Plan automated tasks, such as turning on lights at dusk.

6. Cloud-Based Communication: Users can access and monitor system data remotely thanks to the ESP32 module's data transmission to the cloud. Additionally, the cloud can offer insights into patterns of energy consumption and store historical data for analysis.


Hence, Overall this "Cost-Effective IoT-Based Home Automation System" functions as: The brain of the system, the VSDSquadron Mini board, gathers information from sensors such as motion, temperature, and humidity. After processing this data, it makes choices like turning on lights when it detects motion or modifying fan speed in response to temperature. Through data transmission to the cloud for remote monitoring and command reception from the user interface (web/mobile app), the ESP32 module enables communication. The VSDSquadron Mini receives these commands and uses them to control the relay module that turns appliances on and off. Through the web interface or mobile app, users communicate with the system, scheduling automated actions, managing devices, and monitoring data. This integrated system offers a practical and economical way to control household appliances.

# Features and Benefits of ( CEHA )

a) It Controls the energy management and consumption with power monitoring of all the devices. It controls all the home appliances from the remote directly. So, it is the Remote Control based System which can control the devices from anywhere at anytime easily and making life easier for the individual . 
b) The solution also helps in reducing manual effort and improves efficiency . 
c) This system also optimizes temperature and saving Energy . 
d) It also reduces the cost of the bills and tracks unnecessary usage of the energy which leads to identifying more areas for improvements in energy saving . 
e) This system uses low-cost sensors to track and control the functioning of home/offices appliances for example, Light, Fan,etc. from the remote .

## Some other Key-Features are :- 

- Reducing energy consumption and saving wastage of energy monitoring: This solution is helpful for Person with Disbailities , as they can use remote for controlling the home appliances. 

-Cost-Effectiveness: The implementation of a cost-efficient, open-source hardware architecture (VSD mini RISC-V) enhances the economic feasibility of the system.  -Flexibility: The open-source framework of RISC-V permits extensive customization and fosters the creation of a diverse array of features and integrations.  

-Innovation: This initiative contributes to the expansion of the RISC-V ecosystem and promotes the advancement of novel and inventive home automation solutions. 

-Budget-Friendly: This solution is budget friendly in making this project , as , all the appliance become fully automated, so it makes it easy to control and come under budget as, only sensors are used for making the devices to control automatically. 

-User-Friedly: Any user can use it easily and can control automatically all devices with the help of remote as it interface with the app and wifi module.

# List of Components Required for CEHA System


| Item    | Quantity |
|---------|-----|
|AC Mains Power Supply     | 1  | 
|  4-Channel Relay   | 1  | 
|VSDSquadron mini| 1|
| ESP32 MODULE | 1  |  |
| Touch Sensor | 1 | Display |
| Connecting wires | 1Set |
|2 CH relay5V -240V|1|
| Touch Sensor | 1|
|5v-voltage regulator adaptor| 1|
| Zero PCB | 1|
|Switch | 1 |
| LED bulb | 2|
| Small Fan | 1|
| DHT11 Sensor | 1|
| Case box | 1|

# PIN OUT TABLE  

|Component     	|    Pin/Connection	 |     Connected To|
|----------------|--------------------|-----------------|
|Energy Meter  	|Pulse Output	   |   Optocoupler (Input)|
|Optocoupler(4N35)|	Input	Energy Meter |Pulse Output|
|                 |Output	|VSDSquadron mini GPIO Input Pin (PD2)|
|                |                  |                   |	
|VSDSquadron mini|	GPIO Pin (PD2) 	|LM393 input|
|                |GPIO Pin TX (PD5)|	GPIO Pin RX (16)|
|                | GPIO Pin RX (PD6)|	GPIO Pin TX (17)|
|                |                   |                  |
|ESP32		       |                   |                  |
|                | RX (16)        	|VSDSquadron mini TX (PD5)|
|	        |TX (17)	|VSDSquadron mini RX (PD6)|
|               |              |                          |
|Relay module	|Signal pin	|VSDSquardron mini GPIO Pin PC3|
|               |Vcc	|3.3V/5V (depending on relay)   |
|               |	GND    |	GND            |
|	        |COM	|Power Line (Common)           |
|               |	NO (Normally Open)|	Load(Device Being Controlled)|
|               |	NC (Normally Closed)|	Optional (for fail-safe connections)|
|                |                          |                                       |	
|5 volt adaptaor | 	Phase	|Phase of the energy meter                 |
|                 |	Netural |	Netural of the energy meter         |
|             |	5V	  |VSDSquadron mini|  VCC                                    |
|              |	GND	|VSDSquadron mini | GND                    |                 
|LM393 Comparator |D0      |  VSDSquadron mini   GPIO PD6                |
|                 |5V       |VSDSquadron mini 5V|
|                 |         |VSDSquadron mini GND|
|I2C LCD |	SDA|	vsdsquadron mini GPIO (PC1)|
|            |SCA|	vsdsquadron mini GPIO (PC2)|


# BLOCK DIAGRAM OF THE CEHA SYSTEM 

![block diagram CEHA ](https://github.com/user-attachments/assets/f5a8357d-9aba-4cc0-890a-ebbfae2a339f)

# CIRCUIT DIAGRAM OF CEHA SYSTEM

![circuit diagram of CEHA](https://github.com/user-attachments/assets/339c1629-1405-4375-97f7-8114d61c4cf0)

# Introduction to Arduino IOT Cloud

The Arduino IoT Cloud is an integrated platform designed to facilitate the development and deployment of IoT projects. It enables seamless connectivity and device management providing users with remote control and project monitoring. The projects backbone is the Arduino IoT Cloud which connects the smart energy meter to the internet and enables remote control and real-time data visualization. Because of the Arduino IoT Clouds intuitive interface we can design and manage IoT devices with it. The platform supports many Arduino boards including the popular ESP32 and MKR series which are perfect for Internet of Things applications. The Arduino IoT Cloud allows us to define attributes like cost energy consumption and relay states. These properties have been updated.

# SOURCE CODE OF VSDSQUARDRON MINI AN ESP32 
--------
-----------
# IMAGES OF THE PROJECT
----------
-------------
# DEMONSTRATION VIDEO OF THE PRODUCT Demonstration  
--------
--------

===============================
# ABOUT 
===============


