# DMVPN Lab

## Overview
The **DMVPN Lab** demonstrates the configuration and operation of a **Dynamic Multipoint Virtual Private Network (DMVPN)** using a hub-and-spoke topology with dynamic spoke-to-spoke tunneling. DMVPN is a Cisco technology that combines **Generic Routing Encapsulation (GRE)**, **Next Hop Resolution Protocol (NHRP)**, and **IPsec** to create scalable VPNs. This lab uses **VyOS** routers for the hub and spokes, with **BGP** for dynamic routing, to showcase a **Phase 1 DMVPN** setup where traffic is hub-centric.

This project is ideal for network engineers learning DMVPN or preparing for certifications like **CCNP**. The lab can be run in a virtual environment like **GNS3** or on physical hardware.

## Prerequisites
- **Software**:
  - **VyOS** (version 1.2.0-beta1 recommended) for routers.
  - **GNS3** or a similar network emulator for virtual setups.
  - **Ubuntu Server** with **Cumulus RoH** for BGP routing (optional).
- **Hardware** (for physical setups):
  - Routers supporting GRE, NHRP, and IPsec (e.g., Cisco or VyOS-compatible devices).
- Basic knowledge of **IPsec**, **GRE**, **NHRP**, and **BGP**.
- A GitHub account to clone this repository.

## Getting Started
### Network Topology
!<img width="540" height="149" alt="Image" src="https://github.com/user-attachments/assets/9a469bd7-504a-4a2c-9dab-cade9bdb3336" />


*This diagram shows the lab setup with hosts (h1, h2, h3), routers (R1, R2, R3), and a switch (switch1) connected via Ethernet interfaces.*

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/dmvpn-lab.git
   cd dmvpn-lab
