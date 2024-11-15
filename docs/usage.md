# Usage Instructions

## Door Opening Methods

### 1. Discord Channel
- Join the #door channel on discord.commonshub.brussels
- Type `open` or use `/open` slash command
- Requires channel membership

### 2. API Endpoint
```bash
curl http://localhost:3000/open?secret=YOURSECRET
```
- Requires valid secret key
- Supports programmatic access

## Monitoring and Tracking

### Web Interface
- Access: `http://localhost:3000/`
- Features:
  * Today's visitors
  * Recent door access log
  * Avatar grid

### Logging Endpoints

#### Access Log
```bash
curl http://localhost:3000/log
```
- Displays comprehensive door opening history
- Includes timestamp, user, and agent

#### Device Status
```bash
curl http://localhost:3000/status
```
- Shows connected device information
- Provides network health status

## User Permissions

### Discord Channel Access
- Limited to specific Discord channel
- Requires channel membership
- Role-based access control

### API Access
- Secret key authentication
- Rate-limited access
- Minimal personal information retention

## Common Use Cases

### Authorized Member Access
- Open door via Discord
- Quick, secure entry method

### Remote Management
- API endpoint for programmatic control
- Supports integration with other systems

### Monitoring and Auditing
- Comprehensive access logging
- Visitor tracking
- Detailed system status reporting

## Troubleshooting

### Connection Issues
- Verify network connectivity
- Check Discord bot permissions
- Validate secret key

### Access Denied
- Confirm channel membership
- Verify user roles
- Check API authentication

## Best Practices
- Use secure, unique secret keys
- Rotate credentials regularly
- Monitor access logs
- Limit access to authorized users
