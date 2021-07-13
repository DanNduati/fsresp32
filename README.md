# FSREsp32
## Hardware Components
### 1. Esp32 - Microcontroller
- Get analog force from the FSR sensors
- Publish the FSR sensor data to firebase database every 500 milliseconds

### 2. Force Sensing Resistors(FSR 402) sensors
- Read force data from the patient

#### Interfacing the FSR 402 sensors with the esp32
You need to connect a 10kΩ pull-down resistor in series with the FSR to create a voltage divider circuit. Then the point between the pull-down resistor and the FSR is connected to an ADC input of an Esp32.

<img  height="500" src="images/fsr.png">
## Sofware Components
### 1. Mobile app
- User authentication (login and register)
- Plot line graphs of individual FSR sensor data from the ESP32 

### 2. Firebase database
#### collections
<img  height="500" src="images/firebase_collection.png">
- Store user credentials for mobile app authentication
- Store sensor data from the esp32
