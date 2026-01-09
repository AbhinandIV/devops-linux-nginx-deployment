# Linux + Git Based Application Deployment (DevOps Project)

## Overview
This project demonstrates a production-style deployment of a Node.js application on a Linux (Ubuntu) server using Git for version control, Nginx as a reverse proxy, and systemd for process management.

The focus of this project is infrastructure, deployment flow, and DevOps practices, not application complexity.

---

## Tech Stack
- Ubuntu 22.04
- Node.js
- Git & GitHub
- Nginx (Reverse Proxy)
- systemd (Service Management)

---

## Architecture
Developer Machine 
→ GitHub Repository 
→ Ubuntu Server 
→ Nginx (Port 80) 
→ Node.js Application (Port 3000)

---

## Deployment Flow
1. Developer pushes code to GitHub
2. Code is pulled onto the Linux server
3. Application runs as a systemd service
4. Nginx forwards external traffic from port 80 to port 3000
5. Application restarts automatically on failure or reboot

---

## Key DevOps Concepts Demonstrated
- Linux server administration
- Git-based deployment workflow
- Reverse proxy configuration
- Process management using systemd
- Production-style application exposure

---

## Repository Structure

myapp/
├── app.js
├── nginx/
│ └── myapp.conf
├── systemd/
│ └── myapp.service
└── README.md


---

## How to Run (High Level)
1. Provision an Ubuntu server
2. Install Node.js, Git, and Nginx
3. Clone this repository
4. Copy Nginx config to `/etc/nginx/sites-available`
5. Enable site and reload Nginx
6. Copy systemd service to `/etc/systemd/system`
7. Enable and start the service

---

## Outcome
This project represents a minimum entry-level DevOps deployment, following real-world practices used in production environments.

