---
title: PG19 Radio Frequency 50MHz LC Generator - Repair & Teardown
date: 2023-10-13 15:53:33 +/-TTTT
image: '/images/posts_images/2023-10-13/IMG_20230929_085325.jpg'
tags: [generator, meratronik, analog, radio] # TAG names should always be lowercase
---

![Photo of working generator](/images/posts_images/2023-10-13/IMG_20230929_085325.jpg)

Recently I had the opportunity to repair an early 70s Polish radio frequency generator - PG19. It utilizes a traditional LC oscillator with optional AM modulation from external input or an internal RC generator. Before my repair, there was some signal on the output, but I wasn't able to change the frequency.

## Teardown

The device is very heavy compared to modern DDS equipment. You can access the interior very easily - you just have to remove the top cover and you can see the main parts.

![Top cover](/images/posts_images/2023-10-13/IMG_20230929_085339.jpg)
![Top cover removed](/images/posts_images/2023-10-13/IMG_20230928_134645.jpg)

In the top left corner, you can find the PSU board. Next to the right, under the black cover, there's the main LC generator. Let's go down. Those metal boxes hide adjustable attenuators which allows you to set signal level between 1uV and 3.16V. On the left PCB, there's an audio frequency RC generator which can be used as an AM modulation source.

## Power supply

The power supply is based on a classical circuit utilizing a Zener diode as a reference and two bipolar transistors as the follower. It utilizes 2N3055 as a power transistor. A very popular choice for linear PSU in the 70s.

![PSU](/images/posts_images/2023-10-13/IMG_20230928_095210.jpg)
![PSU](/images/posts_images/2023-10-13/IMG_20230928_123113.jpg)
![PSU](/images/posts_images/2023-10-13/IMG_20230928_123222.jpg)

## RC Generator

RC generator built with BJT utilizes a phase shifter. It provides an AF modulation signal of 400Hz, 1kHz, or 4kHz frequency.

![RC Generator](/images/posts_images/2023-10-13/IMG_20230928_134645(copy).jpg)

## RF LC Generator

PG-19 has 10 ranges and the LC circuit selection mechanism reflects that fact. The principle of operation of the range selection mechanism is simple: the user rotates the drum via a gear, and the contact plates contact the silver-plated pins at the appropriate moment. An auxiliary mechanism ensures the desired contact quality.

![LC Generator](/images/posts_images/2023-10-13/IMG_20230928_122310.jpg)
![LC Generator](/images/posts_images/2023-10-13/IMG_20230928_122337.jpg)
![LC Generator](/images/posts_images/2023-10-13/IMG_20230928_122401.jpg)
![Variable capacitor](/images/posts_images/2023-10-13/IMG_20230928_122743.jpg)
![Variable capacitor](/images/posts_images/2023-10-13/IMG_20230928_122738.jpg)

You can see that the black cover has some screws on top of it. After removing those caps you can access the coils and calibrate your generator. It's a very smart mechanism that makes tunning way easier but still keeps the generator protected from dust.

![Black cover](/images/posts_images/2023-10-13/IMG_20230928_123204.jpg)

# Repair

The problem mentioned at the beginning had a very simple solution. Some mechanical parts were made not of metal, but of texolite. The most problematic turned out to be: the scale cable drive wheel and the sleeve coupling the range switch with the knob. After tightening the screws, the problem disappeared. In addition, the usual problem was cracking potentiometers and switches that needed to be cleaned. At the very end, I carried out measurements which showed that the generator was working properly. There is no problem with modulation and attenuators.

![Disassembled generator](/images/posts_images/2023-10-13/IMG_20230928_122300.jpg)

# Summary

Nowadays, this generator is more of a technical curiosity than a fully functional measuring device. Determining the exact frequency is very difficult, and the stability leaves much to be desired. However, it is worth restoring it to full working order because it is really solidly made and its appearance is pleasing to the eye.