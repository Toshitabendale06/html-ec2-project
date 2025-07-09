# 🌐 Deploying a Static Website on AWS EC2

## 🚀 Project Overview

This project demonstrates how to deploy a basic static HTML/CSS website on an AWS EC2 instance using Apache (or Nginx) web server. It aims to help beginners understand cloud hosting and server setup using Amazon Web Services.

---

## 🎯 Objective

To launch a Linux-based EC2 instance, configure a web server, and host a static website that is publicly accessible over the internet.

---

## 🔧 Tools & Technologies Used

- **Amazon EC2** (t2.micro, Ubuntu/Amazon Linux)
- **Apache Web Server** (or Nginx)
- **HTML & CSS** (basic static site)
- **SSH (MobaXterm/Terminal)** for server access

---

## 🧰 Requirements

- AWS account
- EC2 instance with Ubuntu or Amazon Linux
- Basic HTML/CSS files
- Terminal with SSH support
- Security group allowing port 80 (HTTP)

---

## 📌 Steps Followed

1. **Created an EC2 Instance**
   - Selected Ubuntu/Amazon Linux AMI
   - Chose t2.micro (Free Tier)
   - Configured security group to allow SSH (22) and HTTP (80)

2. **Connected via SSH**
   - Used MobaXterm or terminal to connect:
     ```
     ssh -i "your-key.pem" ec2-user@your-public-ip
     ```

3. **Installed Apache Web Server**
   - For Ubuntu:
     ```
     sudo apt update
     sudo apt install apache2 -y
     ```
   - For Amazon Linux:
     ```
     sudo yum update -y
     sudo yum install httpd -y
     ```

4. **Deployed the Website**
   - Replaced the default `/var/www/html/index.html` with my own `index.html`
   - Restarted Apache server:
     ```
     sudo systemctl start apache2  # or httpd
     sudo systemctl enable apache2
     ```

5. **Accessed Website via Browser**
   - Opened `http://<public-ip>` to view the website

---

## ✅ Output

- A live website hosted on AWS EC2, viewable via public IP
- Apache configured to serve static content from HTML files

---

## 📷 Screenshots

https://github.com/Toshitabendale06/html-ec2-project/blob/main/output.png
---

## 🎥 Video Demonstration

[Click here to watch the video] https://github.com/Toshitabendale06/html-ec2-project/blob/main/toshitarecording-cloud-ec2_nmQyngmg.mp4  
*(Attach or upload your screen recording video here)*

---

## 📚 Learnings

- Basics of cloud infrastructure
- Linux commands for server setup
- Web server configuration (Apache/Nginx)
- Hosting and deploying on AWS

---

## 💬 Author

Toshita Bendale  
3rd Year Student  
GitHub: https://github.com/Toshitabendale06

