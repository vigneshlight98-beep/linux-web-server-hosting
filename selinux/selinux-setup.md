# SELinux Configuration

## Objective
Allow Apache to serve web content from a custom DocumentRoot while SELinux remains enforcing.

## Status
SELinux is running in enforcing mode.

## Configuration
The web content directory `/var/www/companysite` was assigned the
`httpd_sys_content_t` SELinux context to permit Apache access.

## Verification
- getenforce
- ls -Z /var/www/companysite
- curl http://<server-ip>

SELinux was not disabled
