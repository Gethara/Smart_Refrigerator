# Smart Refrigerator System
![image](https://github.com/user-attachments/assets/3fb4443d-8b69-4f83-b720-9390a5bed5bf)
## Overview
This project was developed as part of the Measurements and Instrumentation module in our 4th semester. The smart refrigerator system enhances food management and monitoring by integrating various automated features. The system includes functionalities like an automatic chilled water dispenser, a door contact sensor with a timer, a weight indicator to monitor food levels, and a fruit and vegetable recognition system using machine learning.

## Features
- **Automatic Chilled Water Dispenser**: Dispenses chilled water automatically.
- **Door Contact Indicator with Timer**: Notifies the user when the fridge door has been open for an extended period.
- **Weight Indicator System**: Calibrated weight sensor alerts when food supplies are running low.
- **Fruit and Vegetable Recognition**: Identifies existing fruits and vegetables in the fridge using a custom-trained machine learning model integrated with a Raspberry Pi.
- **LabVIEW Integration**: Manages DAQ cards, automation, and sensor data collection via LabVIEW.

## Components Used
- **LabVIEW**: For programming and controlling the system.
- **Raspberry Pi**: Used for image recognition tasks and system integration.
- **DAQ Card**: For data acquisition and sensor management.
- **Sensors**: Weight sensor, door contact sensor, Water Level sensor.
- **Machine Learning Model**: Trained for fruit and vegetable identification.
- **Chilled Water Dispenser**: Automatically dispenses water.

## System Architecture
1. **LabVIEW DAQ Integration**:
    - DAQ card to collect sensor data from the door, weight sensor, and water dispenser system.
    - Automatic controls for the chilled water dispenser.
2. **Door Contact Timer**:
    - A door contact sensor with a timer to alert if the door is left open for 3 minutes.
3. **Weight Indicator**:
    - Calibrated weight sensors to monitor food supplies and trigger an alert when running low.
4. **Image Recognition (Raspberry Pi)**:
    - Raspberry Pi integrated with a trained machine learning model to recognize and catalog fruits and vegetables in the fridge.
5. **Water Level sensor and Automatic Water Dispenser**:
    - Start the motor and fill the chill water tank when the water level is low, when the water level is higher than a given level the motor stops.
          
## Installation and Setup

### Hardware Setup
1. Assemble the circuit for sensors (weight, door contact).
2. Connect the sensors and actuators to the DAQ card.
3. Set up the Raspberry Pi for image recognition tasks.

### Software Setup
1. **LabVIEW**:
    - Open the LabVIEW project file and configure it for DAQ card integration and automation control.
    - Ensure all sensors are properly calibrated for accurate data acquisition.
2. **Raspberry Pi**:
    - Install necessary Python libraries:
      ```bash
      sudo apt-get update
      sudo apt-get install python3-opencv
      sudo pip3 install tensorflow
      ```
## Usage
- The system automatically dispenses chilled water when the user interacts with the water dispenser.
- The door contact sensor monitors the door status and alerts after 3 minutes if the door is left open.
- The weight indicator monitors food levels and triggers an alert when supplies run low.
- The Raspberry Pi captures images of fruits and vegetables in the fridge and identifies them using the trained model.

## Project Contributions
- **LabVIEW Programming**: Developed control systems for the DAQ card, sensors, and automation.
- **Machine Learning Model Training**: Trained and implemented a model for fruit and vegetable recognition.
- **Raspberry Pi Programming**: Integrated the image recognition model with Raspberry Pi for real-time use.
- **Circuit Design and Sensor Calibration**: Assembled circuits and calibrated sensors for data collection and system accuracy.

## Future Improvements
- Add a mobile app interface to provide real-time updates on fridge contents.
- Integrate a more advanced food spoilage detection system.
- Enhance the weight monitoring system to categorize and track specific food items.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to contribute to this project by forking the repo and submitting pull requests!
