# Arduino-pH-meter
A simple project to measure the pH of a solution using an Arduino-based pH sensor and a web page that plots pH over time.


### Description

- **Hardware**: Arduino, pH probe, and an interface (amplifier) module for the pH probe.  
- **Display**: An HTML/JavaScript page with three tabs (Overview, Wiring & Operation, Visualization). The Visualization tab shows a live (or simulated) pH vs. time chart.  
- **Real vs. Simulated Data**:  
  - Currently, the JavaScript code simulates random pH values as a demo.  
  - Once the project is complete, the simulation will be replaced with real pH measurements from the Arduino (via USB, WiFi, Bluetooth, etc.).

    ![image](https://github.com/user-attachments/assets/43489da2-e76a-4460-8651-32c7ee189d27)
![image](https://github.com/user-attachments/assets/2a203e25-a650-4a4c-928a-2e82aa14bf62)


### Usage

1. **Arduino**  
   - Connect the pH probe to the amplifier (interface) module, then connect the module’s output to an Arduino analog input.  
   - In your Arduino code, read the analog voltage, convert it to pH (using calibration data), and send the measured value to the browser.  
2. **Web Page**  
   - Open the `index.html` (or similar) file in your web browser.  
   - Go to the “Visualization” tab to see the pH vs. time chart (by default, it uses simulated data).

### Calibration

For accurate measurements, calibrate your pH probe with standard buffer solutions (pH 4, pH 7, etc.) and adjust the conversion formula in your Arduino code accordingly.
