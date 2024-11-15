# System Monitoring and Diagnostics

## Real-Time Monitoring Capabilities

### Web Interface Dashboard
- Accessible at `http://localhost:3000/`
- Features:
  * Today's visitors
  * Recent door access log
  * Visual avatar grid
  * System status indicators

## Monitoring Endpoints

### Access Log Endpoint
```bash
GET http://localhost:3000/log
```
- Comprehensive door opening history
- Includes:
  * Timestamp
  * User identifier
  * Opening agent
  * Access method

### Device Status Endpoint
```bash
GET http://localhost:3000/status
```
- Connected device information
- Network health status
- Client connection details

## Logging Mechanisms

### Access Tracking
- Detailed user interaction logging
- Minimal personal information retention
- Timestamped event records

### System Health Logging
- WiFi connection status
- Network connectivity checks
- Hardware interaction logs

## Performance Metrics

### Connection Monitoring
- WiFi signal strength tracking
- Connection attempt statistics
- Reconnection interval analysis

### Resource Utilization
- ESP32 system load
- Network request processing time
- Memory consumption tracking

## Diagnostic Tools

### WiFi Diagnostics
- Signal strength measurement
- Connection attempt logging
- Network interface status

### Hardware Diagnostics
- GPIO pin state tracking
- Relay control monitoring
- LED status indication

## Security Monitoring

### Access Control Tracking
- Authentication attempt logging
- Unauthorized access detection
- IP-based access monitoring

### Anomaly Detection
- Unusual access pattern identification
- Rate limiting violation tracking
- Potential security threat indicators

## Reporting and Alerts

### Log Retention
- Daily log rotation
- Configurable log storage
- Export capabilities

### Alert Mechanisms
- Configurable notification thresholds
- Potential external alert integration
- Critical event highlighting

## Best Practices
- Regular log review
- Implement comprehensive monitoring
- Use minimal, focused logging
- Protect sensitive information
