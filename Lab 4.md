Experiment 4 --> Installing Ubuntu (Ubuntu Desktop and Server), Initial system setup (users, passwords, timezone, and basic configuration) 

Installing Ubuntu (Ubuntu Desktop & Server) and Initial System Setup

Installing Ubuntu is straightforward and involves selecting the appropriate version, configuring partitions, and setting up user accounts.

1. Installing Ubuntu Desktop

Step 1: Download Ubuntu ISO

Get the latest Ubuntu Desktop ISO from ubuntu.com.

Step 2: Create a Bootable USB

Use Rufus (Windows) or Balena Etcher (Mac/Linux) to make a bootable USB.
Boot from the USB by selecting it in BIOS (F2, F12, Esc, or Del).

Step 3: Start Ubuntu Installation

Select Language → Choose English (or preferred language).
Click "Try Ubuntu" or "Install Ubuntu"
"Try Ubuntu" lets you test it without installing.
Choose Keyboard Layout
Connect to Wi-Fi (Optional but recommended)
Select Installation Type
Normal Installation (Includes Office, Media Players, and Utilities).
Minimal Installation (Basic utilities with fewer apps).
Choose Partitioning Method
Erase disk and install Ubuntu (Recommended for beginners).
Something else (For custom partitioning using GParted).
Set Timezone (Auto-detected or choose manually).
Create User Account
Enter your name, username, and password.
Click "Install Now" and wait for installation to complete.
Restart and Remove USB when prompted.

2. Installing Ubuntu Server
   
Step 1: Download Ubuntu Server ISO

Get it from ubuntu.com.

Step 2: Create Bootable USB and Boot

Use Rufus or Balena Etcher, then boot into USB.

Step 3: Install Ubuntu Server

Select Language
Choose Keyboard Layout
Select Installation Type
Use Ubuntu Server (Recommended).
Configure Network
If using DHCP, it configures automatically.
For static IP, enter network details manually.
Set Up Storage
Use entire disk or manually configure partitions.
Set Up User Account
Create an admin user and password.
Select Server Features (Optional)
Install SSH Server if remote access is needed.
Install other services like Docker, LAMP, or Kubernetes if required.
Finish Installation & Reboot

4. Initial System Setup (Post-Installation)

A. Create and Manage Users
Add a new user:

**sudo adduser newuser**

![image](https://github.com/user-attachments/assets/511a12b1-ba90-454f-95cb-3f8b57d5125f)



Grant sudo privileges:

**sudo usermod -aG sudo newuser**

![image](https://github.com/user-attachments/assets/bc3f06fe-457d-4c21-b2cf-c85320122d6b)


List all users:

**cat /etc/passwd**
![image](https://github.com/user-attachments/assets/1c367ec1-1529-47fa-9062-e267a934d3fb)
![image](https://github.com/user-attachments/assets/6c5289f6-8c40-4dac-9cc3-6ca20e0ab920)



B. Set Up Timezone

Check current timezone:

timedatectl
Change timezone (Example: India):

sudo timedatectl set-timezone Asia/Kolkata

C. Update System

Update package lists:

**sudo apt update**
![image](https://github.com/user-attachments/assets/9c2a42bb-eb16-43d3-875d-1f218e23b53c)
![image](https://github.com/user-attachments/assets/2d157d69-58a2-4503-8fb6-76b19c4f5529)




Upgrade installed packages:

sudo apt upgrade -y
![image](https://github.com/user-attachments/assets/df39d13e-fbaa-4b59-a27a-ca28212c7ef5)
![image](https://github.com/user-attachments/assets/31fb1d77-45ef-4c0b-bf53-477078e2d808)




D. Enable SSH (For Remote Access on Ubuntu Server)
Install SSH server (if not installed):

**sudo apt install openssh-server -y**


Start SSH service:

**sudo systemctl enable ssh
sudo systemctl start ssh**
