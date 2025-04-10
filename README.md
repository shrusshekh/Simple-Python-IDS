# 🛡️ Python MAC-Based Intrusion Detection System

This Python intrusion detection system uses Scapy to scan the local network for connected devices and check their MAC addresses against a list of trusted devices. In order to use this code, you need to input your own MAC addresses and IP range using the following commands in Windows command shell:
- ipconfig         # To find your local IP and subnet mask
- getmac           # To find your MAC address

In the code, make the following changes: 
- trusted_macs = [Enter your MAC]                     # Add your trusted MACs
- ip_range = "[Enter your IP range]"                  # Use your subnet range



---

## 🔍 What It Does

- Scans the local network using ARP (Address Resolution Protocol).
- Lists all active devices with their IP and MAC addresses.
- Compares each device's MAC address to a trusted list.
- Prints an alert if a device is not recognized.

---

## ✅ Features

- Works on any local subnet (customizable IP range).
- Trust-based detection using known MAC addresses.
- Good for home or small office network security.

**Note:** This is not an advance IDS, it can be used for **basic** network monitoring. 

---

## ⚙️ Requirements

- Scapy (install with pip)
- pip install scapy
- Run as admin/root (needed to scan the network).
