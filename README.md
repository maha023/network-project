# Emergency Communication Network

## 📌 Description

This project implements a Local Area Network (LAN) without internet connection using GNS3.
It enables communication between devices during emergencies and network outages.

## 🧩 Components

* Router (R1)
* IOSv-L2 Switch
* AlpineLinux-1 (Server)
* AlpineLinux-2 (Client)
* AlpineLinux-3 (Client)

## 🌐 IP Addressing

* AlpineLinux-2: 192.168.1.10
* AlpineLinux-3: 192.168.1.20
* Server: 192.168.2.10
* Router: 192.168.1.1 / 192.168.2.1

## 🔧 Features

* Routing between two networks
* Emergency web server (offline)
* Chat system using netcat (nc)
* Access Control List (ACL) for security

## 🔐 ACL

* Blocks AlpineLinux-3 from accessing the server
* Allows AlpineLinux-2 access

## 💬 Chat System

* AlpineLinux-2: `nc -l -p 1234`
* AlpineLinux-3: `nc 192.168.1.10 1234`

## 🌐 Web Server

* Command: `nc -l -p 80`
* Displays emergency instructions

## 📸 Design

Network topology is included as an image in the repository.

## 🏁 Conclusion

The project demonstrates a reliable offline communication network with routing and basic security.
