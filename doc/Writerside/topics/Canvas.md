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

- Hobby bakers who want fresh bread without hassle
- Bread enthusiasts who want to save time 

## Quality Requirements

| ID                                       | Description                                                                                 |
|------------------------------------------|---------------------------------------------------------------------------------------------|
| <a id="QR_Overheating">QR_Overheating</a> | The bread maker is ensured to not overheat in any situation.                                |
| QR2                                      | There is a fallback connection if WiFi isn't working.                                       |
| QR3                                      | The active recipe is continued after a power breakdown.                                     |
| QR4                                      | It's possible to update the firmware over the air (OTA).                                    |
| QR5                                      | The two microcontrollers don't interfere with each other while baking.                      |
| QR6                                      | The temperature can be controlled from 40 °C to the maximum temperature of the bread maker. |
| QR7                                      | The temperature controller's accuracy falls within +/- 5 °C.                                |

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