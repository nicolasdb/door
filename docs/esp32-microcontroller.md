# ESP32 Microcontroller

## System Overview
Central hardware component managing door control, network connectivity, and system monitoring.

## Hardware Specification
- Model: M5stamp-C3U
- Firmware: MicroPython
- Key Components:
  * WiFi connectivity
  * GPIO pin management
  * Interrupt handling

## Core Modules

### WiFi Management
- Automatic network connection
- Exponential backoff reconnection
- Signal strength monitoring
- Credential secure storage

### Door Control Mechanism
- Relay-based door operation
- Physical button interrupt
- Timeout management
- LED status indication

### Network Interaction
- Periodic API endpoint checking
- Background thread for connection monitoring
- Automatic door opening on server signal

## System Resilience

### Watchdog Timer
- 30-second timeout
- Prevents system hang
- Automatic reset on unresponsive state

### Error Handling
- Graceful connection recovery
- Comprehensive logging
- Systematic reboot strategies

## Safety Protocols
- Always close door on startup
- Immediate door closure during:
  * WiFi connection loss
  * System errors
  * Critical failures

## Configuration
- WiFi credentials management
- Configurable check intervals
- Timeout settings

## Power and Performance
- Low-power design
- Efficient network interaction
- Minimal resource consumption

## Security Considerations
- Minimal network exposure
- Secure credential handling
- Limited connection attempts
