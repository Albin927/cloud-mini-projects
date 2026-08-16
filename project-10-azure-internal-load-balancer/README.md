# Project 10: Azure Internal Load Balancer

## Objective

Created an Azure Internal Load Balancer to distribute HTTP traffic across multiple backend virtual machines within a private Azure network.

## Azure Services Used

- Azure Load Balancer
- Azure Virtual Network
- Azure Virtual Machines
- Backend Pool
- Health Probe
- Load Balancing Rule

## Configuration

### Load Balancer

Name:

`load-balancer`

### Backend Pool

The backend pool contains:

- VM1
- VM2

### Health Probe

Protocol:

`TCP`

Port:

`80`

### Load Balancing Rule

Protocol:

`TCP`

Port:

`80`

### Frontend IP

Private IP:

`10.0.0.4`

## Architecture

```text
                Client
                  |
                  |
            10.0.0.4
          Internal LB
                  |
          +-------+-------+
          |               |
         VM1             VM2
       Port 80          Port 80