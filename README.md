# BeyondMD Projects

## Platform and Technologies
- **Cloud Platform**: AWS
- **Service**: EC2 Instance
- **Containerization**: Docker
- **OS**: Ubuntu
  
## 1. Dockerized "Hello BeyondMD!" Page
[View the Project in the Home Directory](https://github.com/dsilverio123/BeyondMD123/tree/main/home)

### Description
A simple page built with HTML, CSS, and/or JavaScript that displays "Hello BeyondMD!". This web page is dockerized to ensure easy deployment and consistent runtime environment.

### Dependencies
- Docker: `sudo apt install docker.io`
- Docker Compose: `sudo apt install docker-compose`

## 2. System Health Reporting Script for Debian
[View the System Health Project](https://github.com/dsilverio123/BeyondMD123/tree/main/systemhealth123)

### Description
A script tailored for Debian systems to gather and report various system health metrics, including CPU usage, memory consumption, disk utilization, active users, and running processes.

### Dependencies
- sysstat: `sudo apt install sysstat`
- net-tools: `sudo apt install net-tools`

## 3. Ansible Playbook for Docker on Debian Bookworm
[View the Ansible Playbook Project](https://github.com/dsilverio123/BeyondMD123/tree/main/ansible-debian-docker)

### Description
An idempotent Ansible playbook designed for Debian Bookworm systems. This playbook automates the installation and configuration of Docker, ensuring it's executed without unnecessary changes to the system state.

### Dependencies
- Ansible: `sudo apt install ansible`
- Vagrant (Optional, for local testing): `sudo apt install vagrant`

## Firewall Settings
Remember to always ensure your security groups are correctly configured, especially when deploying web-based applications. For the first project, allowing traffic on port 80 is vital:

**Inbound Rules**:
- HTTP (Port 80)
- Custom TCP (Port 19999)
- SSH (Port 22)

> **Note**: Always ensure that your firewall or security groups are configured according to the needs of your application and the best security practices.
