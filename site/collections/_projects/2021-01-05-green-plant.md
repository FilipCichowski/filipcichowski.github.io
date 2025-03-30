---
date: 2025-03-05 05:20:35 +0300
title: EnergoEl Induction Heater Controller 
subtitle: Robust, production ready, for professionals
image: '/images/project-9.jpg'
---

This induction heater controller is meant to automate repetative operations like hardening identical elements, thus providing consistency.

The operation is easy. User can switch between two modes: manual or automatic. In manual mode the heater works while start pedal is pressed.

In automatic mode the heater is turned on during countdown. Countdown occurs only while pedal is pressed. When counter reach 0 it goes back to the value present during pedal press.

Both power & timer value are stored in EEPROM memory and retained during startup. Wear levelling mechanism extend memory lifetime significantly. 

This controller inform user if error occured and allows to delete it.

## Hardware

It's based on Arduino Nano. If MCU breaks client can just connect new Arduino to the computer and you can upload the code remotely.

This clever circuit provide analog output while keeping galvanic separation. It's used for controlling the power with 0-10V voltage. Square wave is reproduced at the emitter of optocoupler's transistor. Integrating circuit provides aproximated DC voltage. Op-amp buffer was added to mitigate the influence of indution heater input impedance.

In order to provide high safety standard ready Meanwell AC/DC converter was used. It's epoxy potted and dedicated for industrial applications.

Ground on the PCB was separated for digital and analog part. 

![Palm trees](/images/image-example-3.jpg)

