# Web Server

## Purpose
Manages authentication, logging, and API endpoints for door control system.

## Architecture
- Node.js Express server
- Discord bot integration
- API endpoint management

## Endpoints

### `/open`
- Door opening mechanism
- Secret-based authentication
- Logs access attempts

### `/check`
- Real-time door status verification
- Returns door state (open/closed)

### `/log`
- Comprehensive access log retrieval
- Tracks door opening events
- Includes timestamp, user, and agent

### `/status`
- System and client status tracking
- Reports connected device information
- Monitors network health

## Features
- User authentication
- Access logging
- Real-time monitoring
- Visitor tracking

## Configuration
- Environment variable management
- Discord bot token setup
- Secret key configuration

## Security Mechanisms
- Secret-based API authentication
- IP tracking and logging
- Rate limiting
- Input validation

## Performance Considerations
- Efficient logging
- Minimal overhead
- Scalable design
