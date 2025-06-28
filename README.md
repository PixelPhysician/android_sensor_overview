# android_sensor_overview

A basic Android app that lists all available sensors on an Android device.
---

## Sensor Overview

The goal of this exercise is to analyze the sensors available on an Android device using the provided sensor overview app.
- Uses Android’s SensorManager to enumerate all available hardware/software sensors
- Works on real devices (e.g., Samsung Galaxy A15)
- Compiles and builds APK using Gradle
- Lists sensors like accelerometer, gyroscope, proximity, orientation 

---

##  Structure

```
androidsensoroverview-main/
├── app/                     # Android application source
├── build.gradle             # Gradle build script
├── gradlew / gradlew.bat    # Gradle wrapper
├── local.properties         # Android SDK path reference
├── settings.gradle          # Gradle settings
└── README.md                # Project documentation (this file)
```

##  Requirements
JDK 17

Gradle

Android Studio

ADB (Android Debug Bridge)

Android SDK

Real Android device (e.g., Samsung Galaxy A15)


## Getting Started

### Installation

```
# Clone repository
git clone https://gitlab.fhnw.ch/david.herzig/androidsensoroverview.git
cd androidsensoroverview-main

# Clean and build
./gradlew clean
./gradlew assembleDebug

app/build/outputs/apk/debug/app-debug.apk
```

---

## Running the App

```
# Plug in Android device and enable developer mode + USB debugging
adb devices
# You should confirm the connection prompt on your phone
adb install -r app/build/outputs/apk/debug/app-debug.apk
```

---



## Exercise Questions & Answers
1. What type/model of Android device are you using?
Samsung Galaxy A15

2. How many sensors are available?
27 sensors detected by the app.

3. List of available sensors
```
1. LIS2DLC12 Accelerometer
2. MXG4300S Magnetometer
3. TCS3701 Light
4. MXG4300S Magnetometer Uncalibrated
5. Significant Motion
6. Step Detector
7. Step Counter
8. Tilt Detector
9. Pick Up Gesture
10. Device Orientation
11. Scontext
12. TCS3701 Light CCT
13. Call Gesture
14. Wake Up Motion
15. TCS3701 Auto Brightness Sensor
16. Pro Tos Motion
17. Device Orientation Wake Up
18. SBM
19. Hover Proximity
20. Touch Pocket
21. SX9385 Grip Sensor
22. Grip Notifier Sensor
23. Motion Sensor
24. Ear Hover Proximity Sensor (ProToS)
25. Camera Light Sensor
26. Samsung GeoMagnetic Rotation Vector Sensor
27. Samsung Orientation Sensor
```


Screenshot from device:

4. Parkinson biomarker
5. The following sensors are especially relevant:
   
Accelerometer (LIS2DLC12) – Tremor detection, bradykinesia

Step Detector / Counter – Gait analysis

Motion Sensor – General movement monitoring


### See Photos attached. :) 
---
by Sarah Deckarm, 2025
