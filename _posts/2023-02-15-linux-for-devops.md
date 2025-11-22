---
title: Essential Linux Commands for DevOps Engineers
date: 2023-02-15 12:00:00 +0530
categories: [DevOps, Cheatsheets]
tags: [linux, bash, terminal, troubleshooting, server-management]
# image:
#   path: /assets/img/headers/linux-header.jpg
#   alt: Linux Terminal
pin: false
math: false
---

As a DevOps engineer, the terminal is your home. Whether you are debugging a crashing container, analyzing HTTP traffic, or managing file permissions, mastery of the command line is non-negotiable.

This guide covers the "daily driver" commands that go beyond basic navigation, focusing on troubleshooting, resource monitoring, and automation.


### `top` / `htop`
Standard for viewing real-time system processes. While `top` is pre-installed everywhere, `htop` provides a friendlier, color-coded interface.

```bash
# Standard top
top

# Interactive, color-coded alternative (install via package manager)
htop

# Check overall disk usage
df -h

# Find which folder is eating your space
du -sh /var/log/*

# Display memory in human-readable format
free -h

# verbose mode to see the handshake and headers
curl -v [https://api.example.com/health](https://api.example.com/health)

# Show only the HTTP response headers
curl -I [https://google.com](https://google.com)

# List processes listening on a specific port (e.g., 8080)
lsof -i :8080

# List all open files by a specific user
lsof -u jenkins

# Show all listening TCP and UDP ports with numeric addresses
ss -tulpn

# Follow a log file in real-time (essential for debugging deployments)
tail -f /var/log/nginx/error.log

# View the last 100 lines
tail -n 100 /var/log/syslog

# Search for "error" in a file, ignoring case (-i)
grep -i "error" application.log

# Recursive search in a directory
grep -r "db_password" /opt/app/config/

# Print only the 1st and 9th columns (e.g., IP and Status Code from access logs)
awk '{print $1, $9}' access.log

# Give execution rights to a script (User: Read/Write/Exec)
chmod u+x deploy.sh

# Standard web permission (Owner: RWX, Group: RX, Others: RX)
chmod 755 /var/www/html

# Change owner to 'ubuntu' and group to 'www-data' recursively
chown -R ubuntu:www-data /var/www/html

```
