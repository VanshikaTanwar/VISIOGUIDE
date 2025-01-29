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

1. Initialization & Power Up:
The system is turned on.The internal components of the VSDSquadron Mini microcontroller are initialized and powered on.

2. Acquisition of Sensor Data:

The ultrasonic sensor receives a trigger signal from the VSDSquadron Mini.After sending out a sound wave, the ultrasonic sensor picks up the reflected echo.The microcontroller determines the distance to the object by timing the sound wave's journey and return. The vibration sensor is constantly watched by the microcontroller for any vibrations that might be signs of movement or intrusion.

3. Processing Data and Making Decisions:

The microcontroller examines the ultrasonic sensor's distance data.It assesses whether the object being spotted is an obstruction (for example, whether it is within a specific range).The microprocessor determines the proper course of action based on the vibration and distance sensor readings.

4. Control of Actuators:

The microcontroller notifies the relays in the event that an obstruction is identified or a security event is initiated (such as vibrations sensed). Relays are used to regulate connected appliances by turning on or off the AC mains electricity.For instance, the system may sound a siren or turn on security lights in the event that an intrusion is detected.

5. Cloud User Interface and Communication:

Sensor data (distance, vibration, etc.) and system status (e.g., alarm triggered) are sent to the cloud using the ESP32 module.Through the cloud, the ESP32 gets commands from the user interface (web-based or mobile app).
The user interface lets users configure automation schedules, view real-time statistics, and remotely control appliances.

6. User Engagement:

Through the online interface or mobile app, users may control devices, keep an eye on sensor readings, and check the status of the system. For automatic actions, they can create timetables and rules (e.g., switch on lights at sunset, adjust thermostat based on temperature).

7.Constant Observation and Reaction:

The system continuously analyzes sensor data and responds to user commands and preset rules.The system continues to function, offering continuous control and protection.



Improving deaf-blind people's mobility and independence is the goal of the VisioGuide project. An ultrasonic sensor built into the system continuously calculates the distance to objects in the user's path. Following processing of this distance data, the VSDSQuadron Mini converts the data into haptic feedback. The user receives real-time feedback from a vibration motor that is connected to the microcontroller. For instance, a change in vibration pattern may indicate a change in direction or a possible hazard, whereas an increase in vibration intensity may indicate an impending obstacle. The user can more safely and confidently navigate their surroundings thanks to this haptic feedback and their preexisting sensory awareness.The effectiveness of the system is further increased by the ability to customize haptic feedback patterns to each user's needs and preferences thanks to the open-source nature of the RISC-V architecture.

Hence, Overall this "Cost-Effective IoT-Based Home Automation System" functions as .

# Features and Benefits of VISIOGUIDE

a) Cost-effective: Projects with a limited budget can make use of the VSDSQuadron Mini since it is an affordable development board.  
b) Open-source: The RISC-V architecture and open-source software tools provide flexibility and customization. 
c) Low Power Consumption: The energy efficiency of the RISC-V core is crucial for battery-powered devices.  
d) Versatility: The board's peripherals and GPIO pins allow for the integration of a wide range of sensors and actuators. 
d) Obstacle Detection: The ultrasonic sensor provides the user with real-time environmental awareness by accurately detecting obstacles in their path.  
e) Haptic Feedback: The vibration motor's unambiguous and educational haptic feedback alerts the user to the presence and proximity of barriers.  
f) Customisable Feedback: To convey different levels of danger, you can change the pattern and intensity of the vibrations. 
g) Compact and Lightweight: The VSDSQuadron Mini's small form factor and lightweight design make it easy to integrate into a portable and user-friendly blind stick.


## Some other Key-Features are :- 

This project makes use of the RISC-V architecture's open-source nature, which permits adaptability and customization. The solution is affordable due to the utilization of the economical VSDSQuadron Mini board. Additionally, the project places a high priority on user-friendliness, making sure that the target audience can easily use and operate the system. 
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


# BLOCK DIAGRAM OF VISIOGUIDE SYSTEM 

![block diagram CEHA ](https://github.com/user-attachments/assets/f5a8357d-9aba-4cc0-890a-ebbfae2a339f)

# CIRCUIT DIAGRAM OF ISIOGUIDE SYSTEM 

![circuit diagram of CEHA](https://github.com/user-attachments/assets/339c1629-1405-4375-97f7-8114d61c4cf0)

# Introduction to Arduino IOT Cloud

The Arduino IoT Cloud is an integrated platform designed to facilitate the development and deployment of IoT projects. It enables seamless connectivity and device management providing users with remote control and project monitoring. The projects backbone is the Arduino IoT Cloud which connects the smart energy meter to the internet and enables remote control and real-time data visualization. Because of the Arduino IoT Clouds intuitive interface we can design and manage IoT devices with it. The platform supports many Arduino boards including the popular ESP32 and MKR series which are perfect for Internet of Things applications. The Arduino IoT Cloud allows us to define attributes like cost energy consumption and relay states. These properties have been updated.

# SOURCE CODE OF VSDSQUARDRON MINI AN ESP32
``` 
#define TOUCH_SENSOR_1  PD2
#define TOUCH_SENSOR_2  PD3
#define OUTPUT_1        PD4
#define OUTPUT_2        PC3

#define ESP_CTRL_1      PC5  // ESP32 control pin for Light 1
#define ESP_CTRL_2      PC6  // ESP32 control pin for Light 2

bool light1 = false;
bool light2 = false;

bool lastTouch1State = LOW;
bool lastTouch2State = LOW;
bool lastESP1State = LOW;
bool lastESP2State = LOW;

void setup() {
    pinMode(TOUCH_SENSOR_1, INPUT);
    pinMode(TOUCH_SENSOR_2, INPUT);
    pinMode(OUTPUT_1, OUTPUT);
    pinMode(OUTPUT_2, OUTPUT);

    pinMode(ESP_CTRL_1, INPUT);
    pinMode(ESP_CTRL_2, INPUT);
}

void loop() {
    // Read touch sensor 1 state
    bool currentTouch1State = digitalRead(TOUCH_SENSOR_1);
    if (currentTouch1State == HIGH && lastTouch1State == LOW) {
        light1 = !light1;  // Toggle light
        digitalWrite(OUTPUT_1, light1);
        delay(300);  // Debounce delay
    }
    lastTouch1State = currentTouch1State;

    // Read touch sensor 2 state
    bool currentTouch2State = digitalRead(TOUCH_SENSOR_2);
    if (currentTouch2State == HIGH && lastTouch2State == LOW) {
        light2 = !light2;  // Toggle light
        digitalWrite(OUTPUT_2, light2);
        delay(300);  // Debounce delay
    }
    lastTouch2State = currentTouch2State;

    // Read ESP32 control 1 state
    bool currentESP1State = digitalRead(ESP_CTRL_1);
    if (currentESP1State == HIGH && lastESP1State == LOW) {
        light1 = !light1;  // Toggle light
        digitalWrite(OUTPUT_1, light1);
        delay(300);
    }
    lastESP1State = currentESP1State;

    // Read ESP32 control 2 state
    bool currentESP2State = digitalRead(ESP_CTRL_2);
    if (currentESP2State == HIGH && lastESP2State == LOW) {
        light2 = !light2;  // Toggle light
        digitalWrite(OUTPUT_2, light2);
        delay(300);
    }
    lastESP2State = currentESP2State;
}


/ done
#include "thingProperties.h"

#define LIGHT_1_CTRL 18  // GPIO for Light 1 control
#define LIGHT_2_CTRL 19  // GPIO for Light 2 control

void setup() {
    Serial.begin(115200);
    initProperties();
    ArduinoCloud.begin(ArduinoIoTPreferredConnection);
    
    pinMode(LIGHT_1_CTRL, OUTPUT);
    pinMode(LIGHT_2_CTRL, OUTPUT);
}

void loop() {
    ArduinoCloud.update();

    // Control VSDSquadron Mini via GPIOs
    digitalWrite(LIGHT_1_CTRL, light1_state);
    digitalWrite(LIGHT_2_CTRL, light2_state);
}

/*
  Since Light1State is READ_WRITE variable, onLight1StateChange() is
  executed every time a new value is received from IoT Cloud.
*/
void onLight1StateChange()  {
  // Add your code here to act upon Light1State change
}
/*
  Since Light2 is READ_WRITE variable, onLight2Change() is
  executed every time a new value is received from IoT Cloud.
*/
void onLight2Change()  {
  // Add your code here to act upon Light2 change
}
/*
  Since Light2State is READ_WRITE variable, onLight2StateChange() is
  executed every time a new value is received from IoT Cloud.
*/
void onLight2StateChange()  {
  // Add your code here to act upon Light2State change
}
``
# IMAGES OF THE PROJECT
----------
-------------
# DEMONSTRATION VIDEO OF THE PRODUCT Demonstration  
--------
--------

===============================
# ABOUT 
===============

```


