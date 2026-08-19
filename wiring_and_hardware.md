# NaviGatr Hardware Wiring Guide

This guide outlines the physical wiring setup for the NaviGatr system, including the GPIO screen, camera extension, fans, power supply, and safety checks.

---

## 📺 GPIO Touchscreen Display

### Overview
- Small 3.5" GPIO touchscreen is used for debugging and demo display
- Connected directly to the Pi 5's GPIO header
- Due to custom 3D printed enclosure, **female-to-female jumper wires** are used to extend the pins cleanly to the display

### Tips:
- Use short jumpers to minimize space
- Match **exact pin numbers**, not wire colors
- Always cross-reference with the official [Raspberry Pi 5 GPIO pinout](https://pinout.xyz)

![alt text](20250506_212509.jpg)

---

## ❄️ Cooling Fan Wiring

### Fan Configuration:
- 2x 30mm fans mounted over the Raspberry Pi compartment
- Connected to GPIO for passive cooling

### Wiring:
- **Red (VCC)** → GPIO Pin 2 or 4 (5V)
- **Black (GND)** → GPIO Pin 6, 9, 14, or 20 (GND)

> ⚠️ Again, don't assume red = 5V. Use a multimeter or double-check the connector orientation.

---

## 📷 Pi Camera Ribbon Extension

### Setup:
- Long Pi Camera ribbon cable (15–30 cm)
- Connects from camera module (front-mounted) to Pi board (rear-mounted)

### Notes:
- Ensure the **metal contact side is facing inward** at both ends
- Fully seat the ribbon cable into the CSI connector and lock it

>![alt text](image.png)

---

## 🔋 Power Supply

### Battery:
- **Anker 10,000 mAh power bank** with USB-C output
- Provides power to:
  - Raspberry Pi 5
  - Coral TPU
  - Fans and GPIO screen

### Notes:
- Cable is routed along the headband crossbeam
- Use a short angled USB-C cable if possible for better fit

---

## 🧠 General Wiring Advice

- Use zip ties or adhesive clips to manage cables inside the headband
- Avoid routing wires across heat-generating areas (e.g., near Pi CPU)
- Add cable slack for Pi-to-screen and Pi-to-camera connectors
- Label jumper ends for quick debugging

---


This wiring setup ensures NaviGatr remains portable, safe, and thermally reliable during real-world use.

