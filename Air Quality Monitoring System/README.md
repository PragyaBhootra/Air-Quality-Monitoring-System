# **Air Quality Monitoring System Using MQ135 Sensor**

## **Overview**
This project implements an air quality monitoring system using the MQ135 gas sensor. It measures air quality in terms of parts per million (PPM) and displays the readings on an LCD. If the air quality exceeds a predefined threshold, an LED blinks, and a buzzer alerts the user.

---

## **Features**
- Measures air quality using the MQ135 sensor.
- Displays real-time air quality readings on a 16x2 LCD.
- Alerts the user with a buzzer and an LED when air quality is poor.
- Serial monitor output for debugging and data logging.

---

## **Components Required**
| Component         | Quantity |
|-------------------|----------|
| Arduino Uno       | 1        |
| MQ135 Sensor      | 1        |
| 16x2 LCD          | 1        |
| Buzzer            | 1        |
| LED               | 1        |
| Resistors         | 2 (220Ω) |
| Breadboard        | 1        |
| Jumper Wires      | As needed |

---

## **Circuit Diagram**
Include or link a circuit diagram that shows how to connect the MQ135 sensor, LCD, buzzer, and LED to the Arduino.

---

## **Setup Instructions**
1. Connect the components as per the circuit diagram.
2. Upload the provided Arduino code to your Arduino board using the Arduino IDE.
3. Open the serial monitor in the Arduino IDE to view real-time air quality data.
4. Observe the LCD display, LED, and buzzer behavior based on air quality.

---

## **Code Explanation**
### **Libraries Used**
- `LiquidCrystal.h`: Controls the 16x2 LCD display.

### **Key Variables**
- `threshold`: Defines the air quality limit beyond which the system triggers alerts.
- `buz`, `led`, `aqsensor`: Pin connections for the buzzer, LED, and MQ135 sensor.

### **Functional Flow**
1. **Setup**:
   - Initializes the pins, LCD, and serial communication.
2. **Loop**:
   - Continuously reads data from the MQ135 sensor.
   - Displays data on the LCD and serial monitor.
   - Activates the buzzer and LED if air quality exceeds the threshold.

---

## **Usage**
1. Connect the system to a power source.
2. Monitor the air quality on the LCD and serial monitor.
3. Respond to alerts when air quality is poor.

---

## **Future Improvements**
- Add Wi-Fi or Bluetooth connectivity for remote monitoring.
- Log air quality data for historical analysis.
- Use a larger display for more detailed information.

---

## **License**
This project is open-source. Feel free to modify and use it for personal or educational purposes.

---

## **Acknowledgments**
- [Arduino Documentation](https://www.arduino.cc/)
- [MQ135 Datasheet](https://www.google.com)

