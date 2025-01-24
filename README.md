# Smart Farming Monitoring System

This repository showcases the **Smart Farming Monitoring System**, a group project that combines IoT and data analysis to create a robust solution for monitoring agricultural environments. The project was developed using WOKWI for IoT simulations and ThingSpeak for data collection and analysis.

## Project Overview

The project aims to implement a smart farming monitoring system with the following goals:
- Develop IoT smart objects using WOKWI.
- Collect and visualize real-time data using ThingSpeak.
- Analyze the collected data using MATLAB Analysis and Visualization.

The system incorporates several smart objects, including sensors for water level, temperature, humidity, soil moisture, and CO₂ levels, along with smart lighting for energy optimization.

---

## Project Structure

### 1. **Smart Object Development**  
The IoT smart objects were simulated using WOKWI, an online IoT development platform. Each smart object is designed to:
- Collect specific environmental data.
- Provide local notifications (e.g., buzzer alerts for water level monitoring).
- Send data to ThingSpeak for real-time monitoring.

#### Example: Water Level Detector  
- **Function**: Monitors water level and triggers a buzzer when water is low.  
- **Simulation**: Built using an ESP32 microcontroller and water level sensor.  
- **Code**: [Source Code](1.%20Pengembangan%20Smart%20Object%20Menggunakan%20WOKWI.docx)  
- **Output**: Detects water level, controls the buzzer, and sends data to ThingSpeak.  

---

### 2. **Data Collection with ThingSpeak**  
- All smart objects send their data to ThingSpeak channels via HTTP or MQTT protocols.
- The collected data is stored and visualized on dashboards for real-time monitoring.

#### Configuration:  
- ThingSpeak channels were set up for each sensor type.  
- Example: The water level detector sends `HIGH` or `LOW` values every 5 seconds to a dedicated channel.

#### Documentation:  
- [Data Collection Details](2.%20Pengumpulan%20data%20menggunakan%20ThingSpeak.docx)

---

### 3. **Data Analysis and Visualization**  
Data analysis was performed using MATLAB's built-in tools in ThingSpeak. Key metrics were extracted to provide insights into environmental conditions:
- Temperature and humidity trends.
- Soil moisture variations.
- CO₂ level monitoring.
- Water level fluctuation patterns.
- Smart lamp brightness adjustments based on LDR sensor readings.

#### Dashboard:  
The dashboard provides real-time visualizations, such as line graphs and bar charts, helping farmers monitor and make informed decisions.

#### Documentation:  
- [Data Analysis and Visualization Report](4.%20Analisis%20data%20menggunakan%20ThingSpeak.pdf)

---

## Group Members
| Name                  | Student ID             |
|-----------------------|------------------------|
| M. Chandra Agoeng P.  | 24/549761/NPA/19958   |
| David Ginola Guterres | 24/549785/NPA/19961   |
| Mayang Adiani E.      | 24/550131/NPA/19969   |
| Fatimah Tuzahra       | 24/550163/NPA/19970   |

---

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/smart-farming-monitoring.git
   ```

2. Set up your WOKWI environment:
   - Import the provided simulation files.
   - Run the simulations and observe the output on the serial monitor.

3. Configure ThingSpeak:
   - Set up your channels as described in the documentation.
   - Update the API keys in the provided code.

4. Analyze and visualize data using ThingSpeak's MATLAB tools.

---

## Files in the Repository

- [`1. Pengembangan Smart Object Menggunakan WOKWI.docx`](1.%20Pengembangan%20Smart%20Object%20Menggunakan%20WOKWI.docx): Development and simulation of IoT smart objects.
- [`2. Pengumpulan data menggunakan ThingSpeak.docx`](2.%20Pengumpulan%20data%20menggunakan%20ThingSpeak.docx): Data collection process using ThingSpeak.
- [`4. Analisis data menggunakan ThingSpeak.pdf`](4.%20Analisis%20data%20menggunakan%20ThingSpeak.pdf): Data analysis and visualization report.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments
We extend our gratitude to Universitas Gadjah Mada for providing the platform and resources to develop this project, as well as our mentors for their invaluable guidance.

---
