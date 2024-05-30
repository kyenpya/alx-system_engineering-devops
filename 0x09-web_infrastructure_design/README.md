# 0x09. Web Infrastructure Design

### Project Details
- **Title**: Web Infrastructure Design
- **Category**: DevOps, SysAdmin, Web Infrastructure

## Concepts
This project will cover the following concepts:
- DNS
- Monitoring
- Web Server
- Network Basics
- Load Balancer
- Server

## Tasks

### 0. Simple Web Stack
**File**: `0-simple_web_stack`

Design a single-server web infrastructure:
- 1 server
- 1 web server (Nginx)
- 1 application server
- 1 application file (code base)
- 1 database (MySQL)
- 1 domain name `foobar.com` pointing to IP `8.8.8.8`

**Explain**:
- What is a server
- Role of the domain name
- DNS record type for `www`
- Role of the web server
- Role of the application server
- Role of the database
- Communication between server and user's computer
- Issues with this infrastructure:
  - SPOF
  - Downtime during maintenance
  - Scalability issues

### 1. Distributed Web Infrastructure
**File**: `1-distributed_web_infrastructure`

Design a three-server web infrastructure:
- 2 servers
- 1 web server (Nginx)
- 1 application server
- 1 load-balancer (HAProxy)
- 1 set of application files
- 1 database (MySQL)

**Explain**:
- Reason for additional elements
- Load balancer's distribution algorithm and its operation
- Active-Active vs. Active-Passive setup
- How a database Primary-Replica cluster works
- Difference between Primary and Replica nodes
- Issues with this infrastructure:
  - SPOF
  - Security issues (no firewall, no HTTPS)
  - Lack of monitoring

### 2. Secured and Monitored Web Infrastructure
**File**: `2-secured_and_monitored_web_infrastructure`

Design a secure and monitored web infrastructure:
- 3 firewalls
- 1 SSL certificate for `www.foobar.com` over HTTPS
- 3 monitoring clients (data collectors)

**Explain**:
- Reason for additional elements
- Purpose of firewalls
- Importance of HTTPS traffic
- Monitoring purpose and data collection
- How to monitor web server QPS
- Issues with this infrastructure:
  - SSL termination at load balancer
  - Single MySQL server for writes
  - Problem with servers having all components

## Repositories
- **GitHub repository**: `alx-system_engineering-devops`
- **Directory**: `0x09-web_infrastructure_design`
  - `0-simple_web_stack`
  - `1-distributed_web_infrastructure`
  - `2-secured_and_monitored_web_infrastructure`

---
