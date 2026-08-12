# Azure Virtual Network Peering

## Overview

This project demonstrates the configuration and management of **Virtual Network (VNet) Peering in Microsoft Azure**.

VNet peering allows two Azure virtual networks to communicate with each other using Microsoft's private network infrastructure.

The project was performed to understand how connectivity can be established between separate Azure virtual networks.

---

## Objective

The main objectives of this project were:

* Understand Azure Virtual Networks
* Understand VNet peering
* Configure peering between virtual networks
* Verify the peering configuration
* Understand private network connectivity in Azure
* Learn how Azure VNets can be connected without requiring a traditional VPN connection

---

## Technologies & Services Used

* Microsoft Azure
* Azure Virtual Network
* VNet Peering
* Azure Virtual Machines
* Azure Networking

---

## Architecture

```text
┌──────────────────────────┐
│   Virtual Network A      │
│                          │
│     Azure VM             │
│                          │
└────────────┬─────────────┘
             │
             │ VNet Peering
             │
┌────────────▼─────────────┐
│   Virtual Network B      │
│                          │
│     Resources            │
│                          │
└──────────────────────────┘
```

VNet peering logically connects the two virtual networks so that resources in the connected networks can communicate using private IP addresses, subject to the configured networking and security rules.

---

## Implementation Overview

### 1. Identify the Virtual Network

The Azure Virtual Network used for the project was accessed through the Azure portal.

The networking configuration was inspected through the VNet settings.

---

### 2. Configure VNet Peering

A peering configuration was created between the virtual networks.

The peering configuration was then synchronized by Azure.

---

### 3. Verify Peering Status

The Azure portal was used to verify the peering configuration.

The peering page displayed the configured peering connection along with its synchronization and connection state.

---

## Result

The VNet peering configuration was successfully created and synchronized.

The Azure portal displayed the configured peering and its current peering status.

## Key Concepts Learned

* Azure Virtual Networks
* VNet Peering
* Private network connectivity
* Azure networking
* Network synchronization
* Inter-VNet communication
* Azure network architecture

---

## Why VNet Peering?

VNet peering is useful when resources located in separate Azure virtual networks need to communicate privately.

It can be used to create larger network architectures while keeping resources organized across different VNets.

---

## Project Significance

This project provided practical exposure to **Azure networking**, moving beyond basic VM deployment and storage management.

It helped demonstrate how Azure resources can be connected through virtual network infrastructure.

---

## Future Improvements

Possible improvements include:

* Deploying VMs in both VNets
* Testing private IP connectivity between the VMs
* Configuring NSG rules for controlled communication
* Exploring hub-and-spoke network architecture
* Testing peering between VNets in different Azure regions
* Exploring Azure VPN Gateway for network connectivity
