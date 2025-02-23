# Automated-Street-Light-Control-System
1. Project Overview
This project automates street light operation based on ambient light levels using an LDR (Light Dependent Resistor) and a microcontroller (Arduino).

At night, the resistance of the LDR increases, turning the lights ON.
During the day, the resistance decreases, turning the lights OFF.
This optimizes energy consumption and reduces manual intervention.

2. Hardware and Software Requirements
Hardware Components:
✅ Arduino Uno – Microcontroller for processing data.
✅ LDR Sensor – Detects ambient light intensity.
✅ Relay Module – Controls the switching of high-power street lights.
✅ LEDs/Bulb – Represents street lights.
✅ Resistors (10kΩ, 1kΩ) – Used for voltage division.
✅ Power Supply (5V DC or 12V for Relays) – Powers the circuit.
✅ Connecting Wires and Breadboard – For circuit connections.

Software Requirements:
✅ Arduino IDE – For writing and uploading the code.
✅ Proteus (Optional) – For circuit simulation.

3. Circuit Diagram and Working
🔗 Circuit Working:
The LDR is connected in a voltage divider circuit.
The microcontroller reads voltage from the LDR and compares it to a threshold.
If the voltage indicates darkness, the relay is activated, switching the light ON.
If it’s bright, the relay is turned OFF.
🔗 Basic Circuit Connections:

LDR → Analog Pin (A0) on Arduino.
Relay Module → Digital Pin (D7) on Arduino.
LED/Bulb → Controlled via Relay Module.

4. Implementation and Testing
✅ Testing Procedure:
Upload the Arduino code using the Arduino IDE.
Place the LDR in a bright environment – The LED/Bulb should be OFF.
Cover the LDR (simulate night) – The LED/Bulb should turn ON.
Observe real-time LDR values in the Serial Monitor.
✅ Observations:
Daytime (Bright Light) → LDR Value High → Light OFF.
Nighttime (Low Light) → LDR Value Low → Light ON.

5. Future Enhancements
🔹 Use IoT (ESP8266/NodeMCU) for remote control.
🔹 Implement solar-powered street lights for energy efficiency.
🔹 Add motion sensors to activate lights only when movement is detected.

🎯 Conclusion
This Automatic Street Light Control System effectively reduces manual efforts and optimizes energy consumption by automatically turning street lights ON/OFF based on ambient light levels.
