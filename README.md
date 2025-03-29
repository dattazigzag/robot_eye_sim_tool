# README

This project consists of 3 components / projects / modules.

It contains parts of a PoC that shows modular tools and blocks that can used by various stakeholders to create simple but rich eye animations and be tested on a desktop based system - thus making it effective for deisgners to deisgn and study design patterns for eye animations on constrained 8x8 addreseable LED matrix displays.

![alt text](_assets/image.png)

👉🏻 [Architechture PDF](<PoC Architechture.pdf>)

🎬 [Video here](https://youtu.be/r1EzEPxQa40)

---

1. [Mic level_ monitor](https://github.com/dattazigzag/mic_level_monitor): A rich python  TUI based terminal application that can be mainly configured to detect volume level changes and send these as triggers via MQTT to a mosquitto broker.  __Usecase:__ _Well, say you want a robot's eye to react to some sound ..._
2. [MQTT_trigg_eye_poc](https://github.com/dattazigzag/mqtt_trigg_eye_poc): A processing application that can mainly receive those MQTT triggers and conduct eye animations and send PGraphics frames over Syphon. __Usecase__: _Well, say you want a standalone tool to try various eye animation patterns in a limited grid ..._
3. [ArtNet DMX Sender](https://github.com/dattazigzag/humanoid_eye_sim): A feature rich processing application that can mainly receive those Syphon [PGraphics](https://processing.github.io/processing-javadocs/core/) frames, downsample them with various pixel processing algorithms and send those data over ArtNet DMX, so that the LED matrix can organize and display them.

