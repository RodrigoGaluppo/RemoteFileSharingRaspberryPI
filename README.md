# Remote File Sharing using Raspberry Pi

## Introduction

Welcome to the README for Remote File Sharing using Raspberry Pi! This project, developed as part of the Operating Systems module within the Bachelor's program in Cybersecurity at Coventry University, aims to demonstrate secure file sharing capabilities using Raspberry Pi devices, OpenMediaVault, and VPN technology. By following this guide, you'll learn how to set up a system that allows for the secure sharing of files over the internet while ensuring data confidentiality.

## Structure

![image](https://github.com/RodrigoGaluppo/RemoteFileSharingRaspberryPI/assets/68329584/51288aea-160c-41ac-b5b4-a9801d845639)


## Overview

The project utilizes Raspberry Pi devices to create a network infrastructure for remote file sharing. We employ OpenMediaVault as the file-sharing platform and implement VPN technology to establish secure connections over the internet. The setup involves three main components:

1. **Raspberry Pi with OpenWrt**: This Raspberry Pi functions as a router and is connected to both the LAN and the internet, serving as the gateway for communication between devices.

2. **Raspberry Pi with OpenMediaVault**: A Raspberry Pi is dedicated to hosting the OpenMediaVault platform, providing shared folders accessible within the local network.

3. **Client Raspberry Pi**: Another Raspberry Pi serves as the client within the server LAN, accessing the shared files from the OpenMediaVault.

4. **Client Devices Through Other LANs**: Other devices that have access to the VPN server, like our desktops from remote locations accessing files securely over the internet.

## Step-by-Step

### 1. Setting up the Raspberry Pi Network Infrastructure

**Conceptual Breakdown:**
- Configure one Raspberry Pi with OpenWrt to act as a router.
- Connect this router to the LAN and the primary router with internet access.
- Ensure proper network configuration to enable communication between devices within the LAN and access to the internet.

### 2. Configuring OpenMediaVault for File Sharing

**Conceptual Breakdown:**
- Install Raspberry Pi OS Lite on a separate Raspberry Pi.
- Install OpenMediaVault on this Raspberry Pi to manage file sharing.
- Set up shared folders and permissions within OpenMediaVault to allow access to files.

### 3. Configuring OpenMediaVault for File Sharing

**Conceptual Breakdown:**
- Install Raspberry Pi OS on a separate Raspberry Pi.
- Connect to the OpenWrt router.
- Access shared files over LAN.

### 4. Establishing a VPN Connection

**Conceptual Breakdown:**
- Configure a VPN server on a cloud-based VPS using OpenVPN.
- Obtain necessary OpenVPN files for client connection.
- Install these files on the Raspberry Pi running OpenMediaVault to make it a client of the VPN server.
- Ensure static assignment of IP addresses for reliable access.

### 5. Get Client Files for Remote Connections

**Conceptual Breakdown:**
- Create client files for remote devices.
- Install OpenVPN client.
- Access shared files over the internet securely.

## Conclusion

This project demonstrates a practical implementation of remote file sharing using Raspberry Pi devices, OpenMediaVault, and VPN technology. By following the steps outlined above, users can set up a secure file-sharing system trhough different LANs in our houses, accessible over the internet while maintaining data confidentiality. It emphasizes the importance of network security and showcases the versatility of Raspberry Pi devices in building innovative solutions.
