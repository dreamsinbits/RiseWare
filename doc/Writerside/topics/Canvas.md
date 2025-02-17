# Canvas

## Value Proposition

Enables users to bake their own recipe with a bread maker.
Furthermore, 
it connects bread makers to the internet,
enabling features like pushing recipes to the bread maker from a baking platform.

## Core Functions

- Loading custom recipes to the bread maker
- Serving as a client for a mobile app and a cloud platform
- Connecting the bread maker to the internet via WiFi
- Providing a Bluetooth connection 

## Key Stakeholders

- Hobbyist bakers who want fresh bread without hassle
- Bread enthusiasts who want to save time 

## Quality Requirements

<include from="RiseWareSnippets.md" element-id="quality-requirements-most-important"/>

See the [](Quality.md) section for more quality requirements and scenarios.

## Core Decisions

- ESP32 as microcontroller:
    - Large community
    - WiFi and Bluetooth
    - GPIOs and analog inputs
- Use of Arduino Framework
    - Large community 
    - Standard
- The original microcontroller of bread maker should still be operational

## Technologies

- C++
- Arduino Framework
- HTML
- PID Controller - [Arduino-PID-Library](https://github.com/br3ttb/Arduino-PID-Library)
- [ElegantOTA](https://github.com/ayushsharma82/ElegantOTA)
- WiFi
- Bluetooth

## Business Context

## Components

## Risks and Missing Information