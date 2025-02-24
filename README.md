# IoT-Security-System

**COMPANY**: CODTECH IT SOLUTIONS

**NAME**: SUKANYA

**INTERN ID**: CT12GFT

**DOMAIN**: INTERNET OF THINGS(IoT)

**BATCH DURATION**: DECEMBER 25TH, 2024 TO FEBRUARY 25TH, 2025

**MENTOR NAME**: NEELA SANTOSH KUMAR

# DESCRIPTION          
This repository contains the Motion Detection System designed using an Arduino Uno and a PIR motion sensor. The project aims to detect motion in its surroundings and provide an alert mechanism using an LED and a buzzer. When motion is detected, the LED lights up, the buzzer sounds an alarm, and a message is displayed on the Serial Monitor. Once the motion stops, the system automatically resets by turning off the LED and stopping the buzzer.                       

This project is useful for home security systems, automatic lighting solutions, and intruder detection systems. It provides a simple yet effective way to monitor motion and trigger alerts accordingly.                         

**Project Overview**                     
The PIR (Passive Infrared) motion sensor detects movement by sensing infrared radiation changes. When a person or an object with heat moves within the sensor's range, it registers the motion and sends a HIGH signal to the Arduino. The Arduino then triggers the LED and buzzer to notify the user of motion detection. When no motion is detected, the system resets by turning the LED off and stopping the buzzer.                            

This project is based on Arduino programming using C++, and the circuit is designed in Tinkercad. The system continuously monitors motion and updates the user via serial communication.                            

**Components Required**                            
To build this project, you will need the following components:                             
Arduino Uno – The microcontroller that processes sensor data and controls output devices                      
PIR Motion Sensor – Detects motion by sensing infrared radiation                                                                  
LED – Indicates when motion is detected                                             
220Ω Resistor – Limits current for the LED to prevent damage                                       
Buzzer – Sounds an alarm to notify motion detection                                          
Breadboard – Helps in making circuit connections                                     
Jumper Wires – For establishing electrical connections between components                                        

**Circuit Diagram and Connections**                                           
PIR Sensor Connections:                                       
VCC → Connect to 5V on Arduino                                      
GND → Connect to GND on Arduino                                      
OUT → Connect to Pin 8 on Arduino                                
 
LED Connections:                                                          
Anode (long leg) → Connect to Pin 9 via 220Ω resistor                                         
Cathode (short leg) → Connect to GND                                           
 
Buzzer Connections:                            
Positive (+) → Connect to Pin 10                          
Negative (-) → Connect to GND                          

**Code Functionality**                                         
The provided Arduino code executes the following functions:                                 

Initialize the PIR sensor, LED, and buzzer during the setup phase                                     
Continuously checks for motion detection using the PIR sensor in the loop                                  
If motion is detected (PIR sensor output = HIGH):                                   

Turns ON the LED                                    
Activates the buzzer                                             
Displays "Motion detected!" on the Serial Monitor                                      
If no motion is detected (PIR sensor output = LOW):                                         
Turns OFF the LED                                           
Stops the buzzer                                          
Displays "Motion stopped!" on the Serial Monitor                                     

**Installation & Usage**                                  
Upload the Code to Arduino:                                   
Open Arduino IDE                                        
Copy and paste the provided code                                     
Select the correct Board and Port                                 
Click Upload to transfer the code to the Arduino                                     

Monitor Serial Output:                         
Open the Serial Monitor in Arduino IDE                                     
Set baud rate to 9600                                                         
Observe motion detection messages in real time                                       

Test the System:                                            
Place the PIR sensor in an area with potential motion                                   
Move in front of the sensor to trigger the LED and buzzer                                             
Stand still or move away to see the system reset                                       

**Applications**                                        
This project has multiple real-world applications, including:                                         

Home Security Systems – Detects unauthorized movement inside a house                   
Automatic Lighting Systems – Turns lights on when motion is detected                                          
Intruder Detection Alarms – Sounds an alarm when an unauthorized person enters a restricted area                           
Smart Home Automation – Enhances energy efficiency by activating devices only when motion is detected                         

**Future Enhancements**                                                                   
This basic motion detection system can be expanded with additional features:                               

Wi-Fi Integration: Connect the system to the Internet using ESP8266 for remote monitoring                     
Mobile App Integration: Use Blynk or Firebase to monitor motion from a smartphone                      
SMS/Email Alerts: Integrate GSM module to send alerts via SMS in case of motion detection                            
Camera Module: Attach an ESP32-CAM to capture images when motion is detected                             

**Output**                               
![Image](https://github.com/user-attachments/assets/275e191c-92d7-4659-a4fc-ec6758a1a8b7)
