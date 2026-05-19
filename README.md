# Multi-Container Web Platform Deployment on AWS EC2

A professional Cloud & DevOps project demonstrating the deployment of a highly secure, multi-container web environment on AWS using Docker and Docker Compose. This project showcases modern system administration, network isolation, and container orchestration skills.

## 🏗️ System Architecture & Infrastructure

The project architecture is built with high isolation and security in mind:
- **Cloud Infrastructure:** AWS EC2 Instance (Ubuntu Server) deployed in a secure VPC.
- **Network Security:** AWS Security Groups configured with strict inbound rules (Restricted SSH & Port Management).
- **Container Networking:** Isolated virtual bridge network (`shahd_network`) ensuring secure internal communication between services.

## 🚀 Technologies Used
- **Cloud:** AWS (EC2, VPC, Security Groups)
- **Containerization:** Docker & Docker Compose
- **Web Server:** Nginx (Latest)
- **Database:** MySQL 8.0 (with persistent volume data storage)
- **Database Management:** phpMyAdmin

## 🛠️ Key Features Demonstrated
- **Port Forwarding (NAT):** Mapping external host ports to internal container ports (`8080` for Web, `8081` for DB Management).
- **Data Persistence:** Using Docker Volumes to ensure database logs and records remain secure even after container updates or server reboots.
- **Service Restart Policies:** Implemented `restart: always` for critical infrastructure backup.

## 💻 How to Deploy
1. SSH into the AWS EC2 Instance:
   ```bash
   ssh -i your-key.pem ubuntu@your-ec2-ip
### 📸 Live AWS Deployment
<img width="1920" height="1020" alt="Screenshot 2026-05-19 093510" src="https://github.com/user-attachments/assets/6a3c7585-2512-43f4-b2dc-72317dbb359a" />

