# sbm20-geiger-counter
ESP32 controlled circuit design outfitting a classic SBM-20 Soviet-era Geiger-Muller tube to detect gamma radiation

This project documents the design and implementation of a geiger counter prototpye using a standard SBM-20 tube. The design process 
consistently focuses on safe high-voltage biasing, analog-digital pulse discrimination and noise reduction to be sensed by an ESP32 Arduino microcontroller board for readings. An earlier analog-focused 
designed was implemented and modeled before being replaced with a simpler and more efficient design using a comparator with hysteresis into the ESP32 GPIO interrupt pin. 
