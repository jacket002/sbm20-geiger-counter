# ESP32 Geiger Counter
EESP32 Geiger Counter

This project documents the design and implementation of an Arduino Nano ESP32 controlled geiger counter circuit outfitting a classic Soviet-era SBM-20 Geiger-Muller tube to detect gamma radiation emissions. The design process consistently manages safe high-voltage biasing, analog-digital pulse discrimination and noise reduction on the hardware side, sensed by the microcontroller for accurate radiation event readings from the environment. 

Initially the geiger counter was designed utilizing NPN transistor switching stages for analog to digital discrimination and buzzer activity–offshoring our device requirements to nearly all analog–before being replaced with the up-to-date comprehensive design using a comparator with selected hysteresis and arduino interrupt service provider (ISR). This had a few trade-offs, one being increased accuracy and noise reduction, but it meant having to get familiar with ESP32 ISR protocols. My view was that this was a much more efficient design choice and a better solution for modern engineering standards. 

I completed this project as a special integration of my interests in nuclear physics with electrical engineering and instrumentation. Practically speaking, this device will allow you to monitor changes in gamma radiation emissions for environmental safety precautions. 
