# Website Hosting using Linux VM & Apache

## Overview

This project demonstrates hosting a template website on a **Linux-based Virtual Machine using the Apache HTTP Server**.

The project was performed to gain practical experience with Linux server environments, Apache web-server configuration, website deployment, and accessing a website through a VM's public IP address.

> **Note:** The website used in this project is a template website used for practicing the hosting and deployment process.

---

## Objective

The objectives of this project were:

* Work with a Linux-based Virtual Machine
* Access and manage a Linux server
* Install and configure Apache HTTP Server
* Deploy website files to an Apache web server
* Make the website accessible through the VM's public IP address
* Understand the basic workflow of Linux-based web hosting

---

## Technologies Used

* Linux Virtual Machine
* Apache HTTP Server
* HTML/CSS Website Template
* Linux Command Line
* Public IP Address
* Web Browser

---

## Architecture

```text
Website Template
       ↓
Linux Virtual Machine
       ↓
Apache HTTP Server
       ↓
HTTP Port
       ↓
Public IP Address
       ↓
Web Browser
```

Apache was used as the web server responsible for serving the website files to clients.

---

## Implementation Overview

The project involved the following general process:

### 1. Linux Virtual Machine

A Linux-based virtual machine was created and configured as the server environment.

### 2. Server Access

The Linux VM was accessed through a remote connection, allowing commands to be executed directly on the server.

### 3. Apache Web Server

Apache HTTP Server was installed and configured on the Linux VM.

Apache acts as the web server that receives HTTP requests and serves the website files to the client.

### 4. Website Deployment

The template website files were placed in the appropriate web-server directory so that Apache could serve them.

### 5. Network Access

The VM was configured to allow web traffic to reach the Apache server.

### 6. Testing

The VM's public IP address was entered into a web browser to verify that the website was accessible externally.

---

## Website

The website used in this project was a pre-existing template website.

The main focus of this project was **server-side deployment and hosting**, rather than frontend website development.

---

## Result

The website was successfully hosted using **Apache on a Linux Virtual Machine** and accessed through the VM's public IP address.


## Key Linux & Server Concepts Learned

* Linux Virtual Machines
* Linux command-line environment
* Apache HTTP Server
* Web-server configuration
* Website deployment
* Public IP addressing
* HTTP-based website access
* Basic server administration

---

## Limitations

The website used in this project was a template rather than a custom-developed application.

The original Linux VM has since been deleted. Therefore, only the available final-result screenshot has been retained in this repository.

---

## Future Improvements

Possible improvements include:

* Deploying a custom-built website
* Configuring Apache Virtual Hosts
* Connecting a custom domain
* Enabling HTTPS using SSL/TLS
* Implementing automated deployment
* Adding monitoring and logging
* Using a reverse proxy
* Deploying multiple websites from the same Linux server
