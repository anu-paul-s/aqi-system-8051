# Air Quality Index (AQI) Monitoring System using MQ-2 and 8051
<img width="1872" height="1004" alt="Screenshot (88)" src="https://github.com/user-attachments/assets/aed57e0f-1bf5-4b32-9910-7773a156c04b" />
<img width="1920" height="1006" alt="Screenshot (89)" src="https://github.com/user-attachments/assets/74c0a782-3ae5-46e5-b692-cf42f9ba1a29" />
<img width="1895" height="1007" alt="Screenshot (90)" src="https://github.com/user-attachments/assets/c5c970d8-2cb6-49d5-9ef7-f0b8c74bb176" />

## 1. Overview
This project implements an Air Quality Index (AQI) monitoring system using the MQ-2 gas sensor and the 8051 microcontroller. It detects gases such as smoke, LPG, and methane, and provides both a numerical AQI value and a qualitative classification. The system categorizes air quality into three levels: Good, Poor, and Dangerous. A buzzer alert is triggered when the AQI exceeds a predefined threshold, indicating hazardous conditions.
## 2. Components Used
- 8051 Microcontroller  
- MQ-2 Gas Sensor  
- Analog-to-Digital Converter (ADC)  
- 16x2 LCD Display  
- Buzzer  
- Resistors and Capacitors  
- Power Supply  
- Connecting Wires  
## 3. Working Principle
The MQ-2 sensor detects gas concentration and generates an analog voltage proportional to gas intensity. Since the 8051 cannot process analog signals directly, an ADC is used to convert the analog signal into digital form. The microcontroller reads the digital data, computes the AQI value, and classifies the air quality based on predefined thresholds: Good, Poor, and Dangerous. If the AQI exceeds the dangerous threshold, a buzzer is activated to alert the user. The AQI value and status are displayed on the LCD.
## 4. AQI Classification
| AQI Level | Air Quality |
|----------|------------|
| Low      | Good       |
| Medium   | Poor       |
| High     | Dangerous  |
*Note: Threshold values can be adjusted based on calibration.*
## 5. Features
- Real-time air quality monitoring  
- Numerical AQI display  
- Air quality classification  
- Buzzer alert for hazardous conditions  
- Simple and cost-effective implementation  
## 6. Software and Tools
- Embedded C  
- Keil uVision  
- Proteus Design Suite  
## 7. Procedure to Run
1. Write the Embedded C program using Keil uVision.  
2. Compile the code and generate the HEX file.  
3. Load the HEX file into the 8051 microcontroller (or Proteus simulation).  
4. Connect the circuit as per the design.  
5. Power the system.  
6. Observe AQI values and air quality status on the LCD.  
7. Verify buzzer activation under high pollution levels.  
## 8. Circuit Description
The MQ-2 sensor outputs an analog signal, which is fed into the ADC. The ADC converts this signal into digital form and sends it to the 8051 microcontroller. The microcontroller processes the data and displays AQI and status on the LCD, and activates the buzzer when the AQI exceeds the threshold.
## 9. Future Enhancements
- IoT-based remote monitoring  
- Improved sensor calibration  
- Data logging and analysis  
- Multi-sensor integration  
## 10. Learning Outcomes
- Interfacing sensors with microcontrollers  
- ADC integration with 8051  
- Embedded C programming  
- Real-time system design  
