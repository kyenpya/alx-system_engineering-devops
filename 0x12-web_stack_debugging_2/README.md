# 0x12. Web stack debugging #2

## Requirements
### General
- All your files will be interpreted on Ubuntu 20.04 LTS.
- All your files should end with a new line.
- A `README.md` file at the root of the folder of the project is mandatory.
- All your Bash script files must be executable.
- Your Bash scripts must pass Shellcheck without any error.
- Your Bash scripts must run without error.
- The first line of all your Bash scripts should be exactly `#!/usr/bin/env bash`.
- The second line of all your Bash scripts should be a comment explaining what the script is doing.

## Tasks
### 0. Run software as another user
**Mandatory**

The root user, on Linux, is the “superuser”. It can do anything it wants, which is both a good and bad thing. It's a good practice to avoid being logged in as the root user to prevent accidental, irreversible commands. Instead, use a privileged user.

For the containers in this project, everything is run under the root user, which can run anything as another user.

#### Requirements
- Write a Bash script that accepts one argument.
- The script should run the `whoami` command under the user passed as an argument.
- Make sure to try your script by passing different users.

### 1. Run Nginx as Nginx

The root user is a superuser that can do anything on a Unix machine. For security reasons, it’s best not to run web servers as root. Instead, run the process as a less privileged nginx user to limit the impact of a security breach.

#### Requirements
- Nginx must be running as nginx user.
- Nginx must be listening on all active IPs on port 8080.
- You cannot use apt-get remove.
- Write a Bash script that configures the container to fit the above requirements.

### 2. 7 lines or less

Using what you did for task #1, make your fix short and sweet.

#### Requirements
- Your Bash script must be 7 lines long or less.
- There must be a new line at the end of the file.
- You must respect Bash script requirements.
- You cannot use ;.
- You cannot use &&.
- You cannot use wget.
- You cannot execute your previous answer file (Do not include the name of the previous script in this one).
