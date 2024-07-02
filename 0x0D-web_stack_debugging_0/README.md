Web Stack Debugging #0

Background Context
The Web Stack Debugging series will train you in the art of debugging. Computers and software rarely work the way we want, which is part of the fun of the job! Being able to debug a web stack is essential for a Full-Stack Software Engineer, and it takes practice to master it.

In this debugging series, you will be provided with broken/bugged web stacks. The final goal is to come up with a Bash script that, once executed, will bring the web stack to a working state. Before writing this Bash script, you should manually figure out what is going wrong and fix it.

Example Scenario
Your server must:

Have a copy of the /etc/passwd file in /tmp
Have a file named /tmp/isworking containing the string OK

Installing Docker
For this project, you will be provided with a container to solve the task. If you wish to experiment with Docker locally, you can install it on your machine. Refer to installation guides for:

Mac OS
Windows
Ubuntu 14.04 (deprecated)
Ubuntu 16.04
Resources
Man or Help:
curl

Requirements
Editors: vi, vim, emacs
Environment: Ubuntu 14.04 LTS
Files: All files should end with a new line and be executable
Bash Scripts: Must pass Shellcheck without any error and run without error
Script Header: First line must be #!/usr/bin/env bash, second line should be a comment explaining the script

Tasks
0. Give me a page!
Task: Get Apache to run on the container and return a page containing "Hello Holberton" when querying the root.

