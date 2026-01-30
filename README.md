# ESP32 Geiger Counter

This project documents the design and implementation of an Arduino Nano ESP32 controlled geiger counter circuit outfitting a classic Soviet-era SBM-20 Geiger-Muller tube to detect gamma radiation emissions. The design process manages safe high-voltage biasing, analog-digital pulse discrimination and noise reduction on the hardware side, sensed by the microcontroller to output accurate radiation event readings.  

Initially the design utilized NPN transistor switching stages for analog to digital discrimination and buzzer activity–outsourcing specified device requirements to almost purely analog front-end–before being replaced with a more comprehensive design using a comparator with selected hysteresis and the arduino interrupt service provider (ISR). This had a few trade-offs, one of which being increased detection accuracy and signal noise reduction, but it meant having to get familiar with ESP32 ISR protocols. My view was that this was a much more efficient design choice and a better standard for modern geiger counter engineering. 

I completed this project after thinking about building something like this for a while to integrate my interests in nuclear physics with electrical engineering and instrumentation. Practically speaking, this device will allow you to monitor changes in gamma radiation emissions for environmental safety precautions. 
