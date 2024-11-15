# Hardware Setup Guide

## Required Components
- M5stampC3U ESP32 Microcontroller
- USB-C Cable for programming
- Relay module
- Power supply
- Connectors type Wago 3-way

## Microcontroller Specifications
### M5stampC3U
- Processor: ESP32-C3
- WiFi: 2.4 GHz
- GPIO Pins: Limited configuration
- Low power consumption

## GPIO Configuration
### Pin Mapping
- **Relay Control**: GPIO Pin 1
- **Built-in Button**: GPIO Pin 9
- **Built-in Status LED**: GPIO Pin 2 (NeoPixel)

## Wiring Diagram
```
M5stampC3U
│
├── GPIO 1 ──► Relay Module
├── GPIO 9 ──► Physical Button
└── GPIO 2 ──► NeoPixel LED
```

## Connection Guidelines
- Ensure proper electrical isolation
- Use appropriate gauge wires
- Implement pull-up/pull-down resistors
- Protect against electrical noise

## Power Considerations
- Stable 5V power supply
- Minimal current draw
- Potential battery/USB power options

## Board Adaptation Warnings
- Pin configurations vary between boards
- Verify electrical compatibility
- Adjust `door_control.py` for different hardware

## Testing Procedures
- Continuity testing
- Voltage level verification
- Interrupt functionality check

## Safety Precautions
- Disconnect power during modifications
- Use anti-static protection
- Avoid short circuits
- Implement physical safety mechanisms
