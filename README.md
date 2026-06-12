# ENCS3320 – Computer Networks Project 2

## Network Design and Implementation Using Cisco Packet Tracer

### Student Information

**Student Name:** Emam Samara
**Student ID:** 1220022
**Course:** ENCS3320 – Computer Networks
**Faculty:** Faculty of Engineering and Technology
**Department:** Electrical and Computer Engineering Department
**University:** Birzeit University
**Semester:** 1252

---

# Project Overview

This project was developed as part of the ENCS3320 Computer Networks course. The main objective is to design, configure, and test a complete computer network using Cisco Packet Tracer.

The project demonstrates practical networking concepts including:

* IP Addressing
* VLSM Subnetting
* Router Configuration
* Static Routing
* DHCP Configuration
* DNS Configuration
* HTTP Web Services
* Email Services
* Network Testing and Verification

The network was designed and implemented according to the project requirements provided by the course instructor.

---

# Network Topology

The implemented topology contains:

### Routers

* Router0
* Router1
* Router2

### Switches

* Switch0
* Switch1

### Servers

* Server0 (Email Server)
* Server1 (Web Server)
* Server2 (DNS + DHCP Server)

### End Devices

* PC0
* PC1
* Laptop0
* Laptop1

The topology allows communication between multiple networks through static routing and provides several network services.

---

# IP Addressing Scheme

### Main Network

192.170.40.0/24

The addressing plan was created using VLSM (Variable Length Subnet Masking).

---

## Network 1

Network Address:

192.170.40.128/26

Default Gateway:

192.170.40.129

Purpose:

Contains:

* PC0
* Server0
* Router0 LAN Interface

---

## Network 2

Network Address:

192.170.40.0/25

Default Gateway:

192.170.40.1

Purpose:

Contains:

* Laptop0
* Server1
* Server2
* Router1 LAN Interface

---

## Network 3

Network Address:

192.170.40.240/29

Purpose:

Router0 ↔ Router1 connection

---

## Network 4

Network Address:

192.170.40.248/29

Purpose:

Router1 ↔ Router2 connection

---

## Network 5

Connected to Router2

Contains:

* Laptop1

---

## Network 6

Connected to Router2

Contains:

* PC1

---

# Router Configuration

All routers were configured with:

* Interface IP Addresses
* Subnet Masks
* No Shutdown commands
* Static Routes

Each router successfully forwards traffic to remote networks.

---

# Static Routing

Static routing was implemented between all routers to ensure full connectivity.

Routing verification was performed using:

* Ping
* Traceroute (tracert)

Successful routing paths were observed across all connected networks.

---

# DHCP Configuration

DHCP service was configured on:

Server2

### DHCP Pool

Pool Name:

Pool_1240494

### DHCP Parameters

Default Gateway:

192.170.40.129

DNS Server:

192.170.40.4

Subnet Mask:

255.255.255.192

Starting Address:

192.170.40.138

### DHCP Client

PC0

PC0 successfully receives its IP address dynamically from the DHCP server.

---

# DNS Configuration

DNS service was configured on:

Server2

### DNS Records

Configured domain:

[www.alawifaisal.com](http://www.alawifaisal.com)

The DNS server resolves the domain name to the Web Server IP address.

DNS functionality was successfully verified using:

* Ping by hostname
* Web Browser access

---

# HTTP Web Server

HTTP service was configured on:

Server1

### Website

Domain:

[www.alawifaisal.com](http://www.alawifaisal.com)

The website contains project information and student details.

Web access was successfully verified from network clients.

---

# Email Service

Email service was configured on:

Server0

### Email Domain

mail.alawifaisal.com

### User Accounts

User 1

Email:
[alawi@mail.alawifaisal.com](mailto:alawi@mail.alawifaisal.com)

Password:
1240

User 2

Email:
[faisal@mail.alawifaisal.com](mailto:faisal@mail.alawifaisal.com)

Password:
0494

### Verification

Email messages were successfully:

* Sent
* Received
* Replied to

between configured users.

---

# Network Testing

The following tests were successfully completed:

### Connectivity Testing

* Ping between routers
* Ping between PCs
* Ping between servers
* Ping between different networks

### DHCP Testing

* Automatic address assignment verified on PC0

### DNS Testing

* Successful hostname resolution

### Web Testing

* Website opened successfully through browser

### Email Testing

* Successful email transmission and reception

### Traceroute Testing

Traceroute successfully displayed routing paths across multiple routers.

---

# Project Features

* Complete VLSM Addressing Design
* Multi-Router Topology
* Static Routing
* DHCP Service
* DNS Service
* HTTP Service
* Email Service
* End-to-End Connectivity
* Cisco Packet Tracer Implementation

---

# Tools Used

* Cisco Packet Tracer
* Static Routing
* DHCP
* DNS
* HTTP
* Email Services
* VLSM Subnetting

---

# Project Status

Completed Successfully

All project requirements were implemented, configured, tested, and verified according to the project specifications.

---

# Author

Emam Samara

Student ID: 1220022

Birzeit University

Faculty of Engineering and Technology

Department of Electrical and Computer Engineering
