# Door Mechanism

## Hardware Specifics: M5stampC3 Configuration
> WARNING: Other ESP32 boards may require different pin mapping
### GPIO Pin Configuration
- **Relay Control**: GPIO Pin 1
- **Physical Button**: GPIO Pin 9
- **Status LED**: GPIO Pin 2 (NeoPixel)

## Board Adaptation Guidelines
- Verify GPIO pin availability on target board
- Check electrical characteristics
- Validate interrupt capabilities
- Adjust `door_control.py` pin definitions accordingly

## Operational Modes

### Automatic Control
- API-triggered opening
- 3-second automatic closure
- Prevents prolonged access

### Manual Interaction
- Physical button toggle
- Debounce mechanism
- Immediate state change

## Status Indicators

### LED Color Codes
- Blue: WiFi Disconnected
- Green: Door Open
- Red: Door Closed
- Flashing Red: Error State

## Safety Mechanisms
- Timeout-based closure
- Interrupt-driven control
- Fail-safe default (closed) state

## Error Handling
- Graceful state management
- Visual error indication
- Logging of state changes

## Configuration Parameters
- Door open duration
- Timeout settings
- Debounce interval

## Board-Specific Considerations
- M5stampC3 has limited GPIO pins
- Power consumption optimization
- Interrupt pin limitations

## Security Considerations
- Minimal physical interface
- Electrical isolation
- Controlled access points
- Pin configuration security
