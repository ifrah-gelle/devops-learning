# devops-learning
My DevOps learning journey
# DevOps Networking Project

## 🚀 Project Overview
This project demonstrates a basic cloud networking setup using AWS and Cloudflare. The goal was to deploy a web server on an EC2 instance and connect it to a custom domain using DNS.

An EC2 instance was launched, NGINX was installed as a web server, and a domain purchased via Cloudflare was configured to point to the server using an A record. The website is successfully accessible through the domain.

---

## 🧱 What I Built
- Launched an AWS EC2 instance (Ubuntu)
- Installed and configured NGINX web server
- Purchased a domain using Cloudflare
- Configured DNS (A record) to point to EC2 public IP
- Enabled HTTP access (port 80) in EC2 security group
- Successfully accessed the web server via custom domain

---

## 🌐 Architecture
User → Domain (Cloudflare DNS) → EC2 Instance → NGINX → Web Page

---

## 📸 Screenshots
All screenshots are stored in:
networking/screenshots/

They include:
- EC2 instance running
- NGINX installation and setup
- DNS configuration in Cloudflare

---

## 🧠 What I Learned
- How DNS works (mapping domain names to IP addresses)
- How to launch and manage EC2 instances in AWS
- How to install and run NGINX on a Linux server
- How web traffic flows from a browser to a server
- Basic cloud troubleshooting techniques

---

## ⚠️ Challenges & Solutions

### Website not loading
Cause: DNS not configured correctly  
Solution: Updated A record with correct EC2 public IP

### NGINX not showing
Cause: NGINX not installed or not running  
Solution:
sudo apt update
sudo apt install nginx -y
sudo systemctl start nginx

### Security group blocking access
Cause: Port 80 (HTTP) not allowed  
Solution: Added inbound rule to allow HTTP traffic

---

## 🛠️ Commands Used
Full list of commands is available in:
networking/Commands.md

---

## 📘 Notes
Detailed learning notes are available in:
networking/Notes.md

---

## 🎯 Conclusion
This project provided a strong foundation in cloud networking, covering DNS configuration, server deployment, and web hosting. It demonstrates practical understanding of how infrastructure components work together in a real-world DevOps environment.
