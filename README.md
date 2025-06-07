# 🌿 Automatic Plant Watering System

This project is an analog circuit-based automatic plant watering system using an LM358 comparator, a soil moisture sensor, and a relay module to control a water pump. The system automatically detects soil dryness and waters the plant without any microcontroller or programming.

## 🛠️ Overview

The goal of this project is to provide a low-cost, energy-efficient, and automatic irrigation solution for small-scale gardening. When the soil becomes dry, the system activates the relay, which turns on the water pump. Once the soil is adequately moist, the pump turns off automatically.

This hardware-based project was designed using **Cicada PCB design software**, and the 3D render shows all the essential components such as the LM358 IC, relay module, variable resistors (for threshold adjustment), and soil probes.

## 🔩 Components Used

| Component            | Description                          |
|----------------------|--------------------------------------|
| LM358 Op-Amp         | Used as a comparator                 |
| Soil Moisture Sensor | Senses moisture in the soil          |
| Relay (5V)           | Switches the pump ON/OFF             |
| BC548 Transistor     | Drives the relay                     |
| 1N4007 Diode         | Flyback protection for relay         |
| Variable Resistors   | Adjust moisture threshold            |
| Water Pump (DC)      | Waters the plant                     |
| Power Supply (12V)   | Provides operating voltage           |

## ⚙️ Working Principle

- The soil moisture sensor outputs an analog voltage based on soil condition.
- This voltage is compared with a reference voltage using the LM358 comparator.
- If the soil is dry (low moisture), the LM358 output goes LOW.
    - This triggers the BC548 transistor.
    - The transistor switches the relay ON.
    - The water pump is activated.
- If the soil is moist, the LM358 output goes HIGH.
    - The relay and pump remain OFF.

## 🔧 Features

- Simple analog design, no code or microcontroller required
- Cost-effective and reliable
- Easy to fabricate PCB
- Real-time plant watering
- Adjustable moisture threshold using potentiometers

## 📷 Project Renders

### ✅ 3D Model of PCB (Designed on Cicada)
![3D View](./images/pcb_render.png)

### ✅ Relay Activation Working
![Relay Working](./images/relay_diagram.jpeg)

### ✅ Moisture Sensor in Soil
![Watering Demo](./images/soil_demo.jpg)

**Developed by:** *Kritish Nagyal*  
Electronics and Communication Engineering (Avionics)  
Central University of Jammu
