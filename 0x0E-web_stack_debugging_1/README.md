# 0x0E. Web Stack Debugging #1

## Description

This project focuses on debugging issues related to a web stack, specifically Nginx configuration. The goal is to ensure Nginx is correctly configured to listen on port 80 of all active IPv4 IPs. The tasks involve using debugging skills and writing Bash scripts to automate the debugging and fixing process.

## Learning Objectives

- Understand network basics related to web servers.
- Develop debugging skills for resolving web stack issues.
- Use Bash scripting to automate server configuration and debugging tasks.

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All files will be interpreted on Ubuntu 20.04 LTS
- All files should end with a new line
- A `README.md` file at the root of the folder of the project is mandatory
- All Bash script files must be executable
- Bash scripts must pass Shellcheck without any errors
- Bash scripts must run without errors
- The first line of all Bash scripts should be exactly `#!/usr/bin/env bash`
- The second line of all Bash scripts should be a comment explaining what the script does
- You are not allowed to use `wget`

## Project Tasks

### Task 0: Nginx likes port 80

- **File:** `0-nginx_likes_port_80`
- **Description:** Fix the issue preventing Nginx from listening on port 80 of the server's active IPv4 IPs. Write a Bash script with the minimum number of commands to automate the fix.
