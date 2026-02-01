# firewalld Configuration

## Objective
Allow HTTP traffic to reach the Apache web server.

## Firewall Status
firewalld service is running.

## Configuration
The HTTP service was permanently allowed through the firewall.

## Commands Used
firewall-cmd --add-service=http --permanent
firewall-cmd --reload

## Verification
- firewall-cmd --list-services
- Browser access to http://<server-ip>

