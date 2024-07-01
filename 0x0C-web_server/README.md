Web Server Project

Concepts
Child Process: Understanding the concept and how it is applied in web servers.
Background Context
This project involves setting up and configuring a web server. Some tasks will be graded on:

Web-01 server configuration.
Bash scripts to automate the configuration of an Ubuntu machine.

Requirements
Editors: vi, vim, emacs
Environment: Ubuntu 16.04 LTS
Files: End with a new line, README.md is mandatory, all Bash scripts must be executable.
Bash Scripts: Pass Shellcheck (version 0.3.7) without errors.
Script Header: First line must be #!/usr/bin/env bash, second line should be a comment explaining the script.
Restrictions: Cannot use systemctl for restarting a process.

Tasks
0. Transfer a file to your server
Script: 0-transfer_file
Parameters: Path to the file, server IP, username, path to SSH private key.

1. Install nginx web server
Script: 1-install_nginx_web_server
Requirements:
Install nginx on web-01 server.
Nginx listens on port 80.
Returns "Hello World!" when queried with curl.

2. Setup a domain name
Domain Registration: Use .TECH Domains.
Requirements:
Provide only the domain name (e.g., myschool.tech).
Configure DNS with an A entry pointing to web-01 IP address.
Enter domain in the Project website URL field.

3. Redirection
Script: 3-redirection
Requirements:
Configure Nginx to redirect /redirect_me to another page with a 301 status.

4. Not found page 404
Script: 4-not_found_page_404
Requirements:
Configure Nginx to return a custom 404 page with "Ceci n'est pas une page".
