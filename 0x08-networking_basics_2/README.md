Networking Basics #2
Description
This project delves into more advanced networking concepts, covering topics such as localhost, 0.0.0.0, the hosts file, and netcat usage. By understanding these concepts, we gain insights into network configurations and troubleshooting.

Learning Objectives
Upon completion of this project, you should be able to explain the following without relying on external sources:
The concept of localhost and its significance
The purpose of 0.0.0.0 in networking
How the hosts file is used in network resolution
How to display active network interfaces on a machine

Requirements
Allowed editors: vi, vim, emacs
Bash script files interpreted on Ubuntu 20.04 LTS
All files end with a new line
Mandatory README.md file
All Bash scripts must be executable
Bash scripts must pass Shellcheck (version 0.7.0) without errors
First line of all Bash scripts: #!/usr/bin/env bash
Second line of all Bash scripts: Comment explaining script functionality

Tasks
0. Change your home IP
Write a Bash script that configures an Ubuntu server to resolve localhost to 127.0.0.2 and facebook.com to 8.8.8.8.

1. Show attached IPs
Write a Bash script that displays all active IPv4 IPs on the machine it's executed on.

2. Port listening on localhost (Advanced)
Write a Bash script that listens on port 98 on localhost. This script can be useful for debugging socket connection issues, testing firewall rules, and more.
