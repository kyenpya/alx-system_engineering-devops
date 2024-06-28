# 0x0A. Configuration Management

## Description
This project focuses on configuration management using Puppet. You'll learn to automate various tasks such as file creation, package installation, and process management in an infrastructure environment.

## Background Context
When I was working for SlideShare, I worked on an auto-remediation tool called Skynet that monitored, scaled, and fixed Cloud infrastructure. I used a parallel job-execution system called MCollective, which allowed me to execute commands on one or multiple servers at the same time. One day, due to a bug in my code, I accidentally sent a command to terminate all servers instead of a selected few. This resulted in shutting down 75% of SlideShare's document conversion environment. Thanks to Puppet, we were able to restore our infrastructure to normal operation in under an hour, which would have been much longer if done manually.

[That was me ^_^‘](https://x.com/devopsreact/status/836971570136375296)

## Requirements
### General
- All your files will be interpreted on Ubuntu 20.04 LTS
- All your files should end with a new line
- A `README.md` file at the root of the folder of the project is mandatory
- Your Puppet manifests must pass puppet-lint version 2.1.1 without any errors
- Your Puppet manifests must run without error
- Your Puppet manifests' first line must be a comment explaining what the Puppet manifest is about
- Your Puppet manifests files must end with the extension `.pp`

### Note on Versioning
Your Ubuntu 20.04 VM should have Puppet 5.5 preinstalled.

#### Install Puppet
```sh
$ apt-get install -y ruby=1:2.7+1 --allow-downgrades
$ apt-get install -y ruby-augeas
$ apt-get install -y ruby-shadow
$ apt-get install -y puppet


Tasks
0. Create a file
File: 0-create_a_file.pp
Description: Using Puppet, create a file in /tmp with the following requirements:
File path is /tmp/school
File permission is 0744
File owner is www-data
File group is www-data
File contains I love Puppet

1. Install a package
File: 1-install_a_package.pp
Description: Using Puppet, install flask from pip3 with the following requirements:
Install flask
Version must be 2.1.0

2. Execute a command
File: 2-execute_a_command.pp
Description: Using Puppet, create a manifest that kills a process named killmenow with the following requirements:
Must use the exec Puppet resource
Must use pkill
