# 0x0F. Load Balancer

## Description

This project focuses on configuring a load balancer to distribute traffic across multiple web servers. By doing this, we aim to improve the reliability and scalability of our web stack. The project involves writing Bash scripts to automate the configuration of new Ubuntu servers to meet the specified requirements.

## Learning Objectives

- Understand the concept of load balancing and HAproxy.
- Configure web servers to handle more traffic and ensure redundancy.
- Use Bash scripts to automate server configuration.

## Project Tasks

### Task 0: Double the number of webservers

- **File:** `0-custom_http_response_header`
- **Description:** Configure `web-02` to be identical to `web-01`. Add a custom Nginx response header `X-Served-By` with the hostname of the server. Write a Bash script that configures a brand new Ubuntu machine to meet these requirements.

### Task 1: Install your load balancer

- **File:** `1-install_load_balancer`
- **Description:** Install and configure HAproxy on `lb-01`. Configure HAproxy to send traffic to `web-01` and `web-02` using a round-robin algorithm. Ensure HAproxy can be managed via an init script. Write a Bash script that configures a new Ubuntu machine to meet these requirements.
