# ECE 528/L - Robotics and Embedded Systems with Lab
**CSU Northridge**

**Department of Electrical and Computer Engineering**

## Bluetooth Low Energy (BLE) Lab
The Bluetooth Low Energy (BLE) lab interfaces with the following:

* User LEDs of the TI MSP432 LaunchPad
* Pololu Gearmotor with Encoder - [Product Link](https://www.pololu.com/product/3675)
* Adafruit Bluefruit LE UART Friend - Bluetooth Low Energy (BLE) Module - [Product Link](https://www.adafruit.com/product/2479)

## Overview
Build a C project to create a line follower robot that will drive along a line maze course using the 8-Channel QTRX Sensor Array module. Utilize a finite state machine and interrupts to handle sensor and motor control.

## Compontents Used
    - MSP432 LaunchPad
    - USB-A to Micro-USB Cable
    - TI-RSLK MAX Chassis
    - Pololu Gearmotor with Encoder
    - Adafruit Bluefruit LE UART Friend - Bluetooth Low Energy (BLE) Module

## Pre-Lab Assignment
1. What is Bluetooth Low Energy(BLE)? How does it differ from regular Bluetooth in terms of power consumption and range?
    BLE is an extension to Bluetooth 4.x, and is used for low latency and fast transactions. Main Bluetooth is good for audio and video applications but BLE is used for IoT connections. BLE also uses less power but also has a less range compared to normal Bluetooth

2. What does GAP stand for and what is its purpose? What is the difference between Peripheral and Central devices in the context of BLE?
    GAP stands for Generica Access Profile. GAP controls connections and advertising in Bluetooth. A Peripheral devices are small, low power, resource constrained devices that can connect to a more powerful central device. Central devices are usually the mobile phone or tablet, which have more processing power and memory.

3. What is GATT in BLE, and how does it structure data exchange between connected devices? Provide definitions for the following: Profile, Service, Characteristic.

GATT is Generic Attribute Profile. It is used to send and receive short pieces of data known as "attribues".
    -Profile : pre-defined collection of Services that has been compiled by either the Bluetooth SIG or by the peripheral designers.
    -Services : Used to break data up into logical entities.
    -Characteristics : Specific Chunks of data

4. What is an advertising packet in BLE and what information can it contain?
    The advertising payload is constantly transmitted and lets the central devices in range know that it exists.

5. What is a UUID used for in BLE nad why are 128-bit UUIDs used? 
    UUID is a number to identify information in computer systems. 


## Analysis and Results
Issues were found with the button not releasing initially but that was due to recieving too many packets in the buffer and not capturing the correct amount.

## Known Issues or Limitations



## References
