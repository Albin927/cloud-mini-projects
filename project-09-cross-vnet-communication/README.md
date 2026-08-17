# Cross-VNet Communication with a Friend's VNet

## Overview

This project demonstrates the practical implementation of **Azure Virtual Network (VNet) Peering** by connecting my Azure Virtual Network with a friend's Azure Virtual Network.

After establishing the peering connection, communication between virtual machines in the two different VNets was tested using private IP addresses.

The connectivity was further verified by accessing a shared folder between the virtual machines and exchanging a test file.

---

## Objective

The main objectives of this project were:

- Connect two separate Azure Virtual Networks
- Configure VNet Peering between the VNets
- Establish private communication between virtual machines
- Test connectivity using private IP addresses
- Verify connectivity using the `ping` command
- Access a shared folder between the connected VMs
- Demonstrate practical cross-VNet communication

---

## Technologies & Services Used

- Microsoft Azure
- Azure Virtual Network (VNet)
- VNet Peering
- Azure Virtual Machines
- Private IP Addressing
- Windows
- ICMP / Ping
- Windows Network File Sharing

---

## Architecture

```text
              My Azure VNet
             ┌──────────────┐
             │              │
             │    My VM     │
             │              │
             └──────┬───────┘
                    │
                    │
              VNet Peering
                    │
                    │
             ┌──────▼───────┐
             │              │
             │ Friend's VNet│
             │              │
             │ Friend's VM  │
             │  10.2.1.4    │
             │              │
             └──────────────┘