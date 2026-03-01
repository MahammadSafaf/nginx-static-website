# Nginx Static Website Deployment Project

## 📌 Project Overview
This project demonstrates deployment of a static website using Nginx on Ubuntu Linux and managing the project using Git and GitHub.

The objective of this project was to understand:
- Web server installation
- Nginx configuration
- Linux file permissions
- Port verification
- Version control using Git
- Remote repository management using GitHub

---
## 🛠 Technologies Used
- Ubuntu Linux
- Nginx Web Server
- Git
- GitHub

---
## 📂 Project Directory Structure
Project Path:
/var/www/myproject

Files:
- index.html
- README.md

---
## ⚙️ Implementation Steps

### 1️⃣ Installed Nginx
sudo apt update
sudo apt install nginx

### 2️⃣ Created Project Directory
sudo mkdir -p /var/www/myproject

### 3️⃣ Configured Nginx Root
Edited:
/etc/nginx/sites-available/myproject

Changed root to:
/var/www/myproject

Restarted Nginx:
sudo systemctl restart nginx

---
### 4️⃣ Verified Deployment
Tested using:
curl http://localhost

Verified port 80:
sudo ss -tulpn | grep :80

---
### 5️⃣ Version Control Using Git
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <repository-url>
git push -u origin main


Verified commit history:
git log --oneline

---
## ✅ Project Outcome
- Successfully deployed static website using Nginx
- Configured custom root directory
- Verified service status and listening ports
- Managed project with Git
- Pushed code to GitHub repository

---
## 📷 Proof of Work
Commands used:
- sudo systemctl status nginx
- sudo ss -tulpn | grep :80
- git log --oneline

---
## 🚀 Future Improvements
- Deploy on cloud server (AWS / Azure / GCP)
- Configure domain name
- Enable HTTPS using SSL
- Automate deployment using CI/CD

---
## 👨‍💻 Author
Mahammad Safaf

---
## 📂 Project Directory Structure
Project Location: /var/www/myproject

Files inside project:
- index.html
- README.md
- .git directory
