# Project 11: Azure Public Load Balancer

## Objective

Configured and tested an Azure Public Load Balancer to distribute incoming HTTP traffic across multiple backend virtual machines.

## Azure Services Used

- Azure Load Balancer
- Azure Virtual Machines
- Azure Virtual Network
- Backend Pool
- Health Probe
- Load Balancing Rule
- Public IP Address

## Configuration

### Load Balancer

Created an Azure Load Balancer with a public frontend IP address.

### Backend Pool

The backend pool contains multiple virtual machines that host the web application.

- VM1
- VM2

### Health Probe

Configured a health probe to check the availability of the backend web servers.

**Protocol:** TCP  
**Port:** 80

### Load Balancing Rule

Configured an HTTP load-balancing rule to distribute incoming traffic to the backend virtual machines.

**Protocol:** TCP  
**Frontend Port:** 80  
**Backend Port:** 80

## Architecture

```text
                   Internet
                       |
                       |
                Public IP Address
                       |
                Azure Load Balancer
                       |
              +--------+--------+
              |                 |
             VM1               VM2
           Port 80           Port 80
              |                 |
        Web Server          Web Server