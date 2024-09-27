# SignGlove: A Wearable Communication Device for Paralyzed Patients

**SignGlove** is an innovative wearable glove designed to bridge the communication gap for paralyzed patients, enabling them to express their wants and needs through hand signals. It allows caretakers to understand and respond to individuals with limited mobility in a personalized and configurable manner.

## Overview

- **Communication Aid**: SignGlove translates specific hand signals into messages, allowing paralyzed individuals to communicate with their caregivers.
- **Customizable**: The glove is configurable to suit the unique hand movements of each user. It can interpret signals based on both finger flexions and palm orientations, providing up to 64 possible hand gestures.
- **Wi-Fi Connectivity**: Transmits hand signals over a Wi-Fi network to a caregiver’s device for quick and efficient communication.

## Inspiration

SignGlove was inspired by the **SignAloud** project, developed by Navid Azodi and Thomas Pryor from the University of Washington, which translates American Sign Language into text or speech. Additionally, the idea of communication through non-verbal cues, as portrayed by Don Hector Salamanca in *Breaking Bad*, influenced the creation of this system to help individuals convey their needs.

## How It Works

1. **Flex Sensors**: Flex sensors are attached to each finger and capture resistance changes when fingers are flexed or extended. These signals are processed by the **ESP32 Development Board**.
2. **MPU6500 IMU**: The Inertial Measurement Unit tracks the orientation of the hand, providing context for signal interpretation (e.g., palm up or down).
3. **OLED Display**: A 128x64 OLED display shows real-time readings from the sensors, allowing users to calibrate and fine-tune the system.
4. **Configurable Firmware**: Caregivers can generate customized firmware for SignGlove by using a web application that tailors the system to each user’s hand signals.

### Components

- **ESP32 Development Board**
- **MPU6500 IMU** (for hand orientation detection)
- **128x64 OLED Display** (for user interface and calibration)
- **Flex Sensors** (attached to each finger to detect movement)
- **Wi-Fi** (for transmitting hand signals to a caregiver’s device)

## Configuration and Calibration

The glove can be tailored to each individual by calibrating the flex sensor readings and hand orientation. Through the **OLED screen**, users can view real-time readings and adjust the device to match their specific hand movements.

Caregivers can use a web application to input the user’s movements and generate a unique firmware tailored to those hand signals. This firmware is uploaded to the SignGlove device, ensuring a personalized experience for the user.

## Web Application

The SignGlove system includes a **web app** where caregivers can:

- Input specific hand signals and orientations for customization.
- Generate unique firmware based on the user's gestures.
- Upload the generated firmware to the SignGlove, personalizing the communication experience for the patient.

### [Add Blog Link Here]

## Future Enhancements

We are continually working on improvements to SignGlove. Planned updates include:

1. **Pressure-Sensitive Conductive Sheets**: Transitioning from flex sensors to pressure-sensitive conductive sheets like Velostat for enhanced control and accuracy.
2. **Compact PCB Design**: Designing a custom PCB to consolidate the ESP32, MPU6500, and OLED Display into a single compact unit for easier embedding into the glove.
3. **Increased Testing**: Conducting more extensive user testing to refine the firmware and improve the system's reliability and ease of use.

---

**Visit the Blog:** [Blog](https://mbedsyst.blogspot.com/2023/06/signglove-bridging-communication-gap.html)

**Web Application:** The web application for customizing SignGlove firmware can be accessed [Here](https://hani-2020.github.io/SignGlove/).
