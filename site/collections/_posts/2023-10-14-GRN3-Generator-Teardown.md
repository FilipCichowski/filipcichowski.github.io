---
title: USSR Generator GRN-3 250kHz - Repair & Teardown
date: 2023-10-15 04:13:33 +/-TTTT
image: '/images/posts_images/2023-10-14/IMG_20231005_091619.jpg'
tags: [generator, analog, radio, ussr] # TAG names should always be lowercase
---

![Photo of working generator](/images/posts_images/2023-10-14/IMG_20231005_091619.jpg)

## Background

Soviet electronics always contained some unusual solutions. Despite its poor quality I find tearing Russian devices very entertaining. That's why I decided to show you the interior of this low-frequency generator.

The front panel design reminds me of the [C1-118](https://danyk.cz/c1-118_en.html) & [C1-112](https://www.radiomuseum.org/r/unknown_c1_112a_s1_112.html) oscilloscopes. It's a shame that the generator has a different width than those scopes because it would create a really nice set.

Enough talking, let's tear it down!

## Ah, the quality of Russian electronics...

Both parts of the enclosure are so supple that you can bend them easily. The plastics don't fit together, putting them together is almost a miracle.

![Bottom part of enclosure](/images/posts_images/2023-10-14/IMG_20231005_091730.jpg)

After opening we can see entire device build on single PCB.

![PCB inside](/images/posts_images/2023-10-14/IMG_20231004_204319.jpg)
![PCB inside](/images/posts_images/2023-10-14/IMG_20231004_210257.jpg)

I decided to blindly replace the electrolytic capacitors, because I know that the Russian capacitors were of terrible quality.

I took off the plastic cover of the mains switch for a moment to see what was under it. I saw very poorly soldered wires that were about to break off. I repaired the connections with some fresh tin, because the whole thing posed a threat to the user's life.

![Mains switch](/images/posts_images/2023-10-14/IMG_20231004_211558.jpg)

## Repair

Well, since I managed to deal with the most serious faults, I decided to check the quality of the signal from the generator. As you can see in the oscillogram, the sine wave had its peaks cut off.

![Sine wave with cut peaks](/images/posts_images/2023-10-14/IMG_20231004_212834.jpg)

Fortunately, it turned out that the designer had included a potentiometer on the board to set the operating point of the signal amplifier, which made it possible to easily correct this defect.

![Operating point potentiometer](/images/posts_images/2023-10-14/IMG_20231004_213852.jpg)
![Expected sine](/images/posts_images/2023-10-14/IMG_20231004_213003.jpg)

## Calibration

Additionally, I decided to set the duty of the rectangular waveform to 50%.

![Duty potentiometer](/images/posts_images/2023-10-14/IMG_20231004_214008.jpg)
![Expected square wave](/images/posts_images/2023-10-14/IMG_20231004_214019.jpg)

The generator frequency is selected in steps. We choose the frequency basis and the multiplier. I calibrated the device so that the frequency set by the switches coincided with reality.

![Frequency counter display](/images/posts_images/2023-10-14/IMG_20231004_215614.jpg)
![Frequency counter display](/images/posts_images/2023-10-14/IMG_20231004_215624.jpg)
![Frequency counter display](/images/posts_images/2023-10-14/IMG_20231004_215634.jpg)

## Summary

Nowadays, the parameters of this generator are not impressive, but it can still be used to test audio devices.

