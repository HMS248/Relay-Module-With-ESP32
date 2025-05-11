# Relay-Module-With-ESP32

## Project Description

This project contains Arduino code for an ESP32 microcontroller to control a relay module, which in turn controls lights, to create a variety of blinking patterns.  The code is designed to demonstrate different ways to manipulate a relay for visual effects using a simple ESP32 and relay setup.

## Hardware

* ESP32 Development Board
* Single-channel or 2-relay module
* Wiring to connect the ESP32 to the relay module
* Light source controlled by the relay

## Wiring

The ESP32 is connected to the relay module as follows:

* ESP32 GPIO pin (e.g., GPIO 25) -> Relay module IN pin
* ESP32 3.3V or 5V -> Relay module VCC
* ESP32 GND -> Relay module GND
* Relay module COM, NO, and NC connected to the light source

## Code Description

The Arduino code provides the following functionality:

* **`blinkPattern(int blinkCount, int blinkDelay)`:** This function controls a single blinking pattern with a specified number of blinks and a delay for the ON and OFF states.
* **`speedTransition(int startDelay, int endDelay, int steps, int count)`**: This function generates a sequence of blinking patterns with a gradual change in blinking speed.
* The `loop()` function contains a sequence of 20 different blinking patterns, demonstrating various speeds, durations, and combinations.  Patterns include:
    * Quick blinks
    * Slow blinks
    * Single flashes
    * Alternating speeds
    * Morse code-like patterns
    * Increasing/decreasing speed transitions

## Usage

1.  Connect the ESP32 to the relay module and the light source as described in the Wiring section.
2.  Upload the Arduino code to the ESP32 using the Arduino IDE.
3.  Observe the light source as it displays the different blinking patterns.

## Author

* hms_tech

## License

* Specify the license for your project.  For example:  MIT License

