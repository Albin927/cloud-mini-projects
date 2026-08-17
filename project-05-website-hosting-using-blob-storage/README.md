# Website Hosting using Azure Blob Storage

## Overview

This project demonstrates hosting a **static website using Azure Blob Storage**.

The project was completed to understand how a website can be deployed without using a traditional virtual machine or web server. Azure Blob Storage provides static website hosting functionality that can serve HTML, CSS, JavaScript, and other static website files.

> **Note:** The website used in this project was a pre-existing template website used for practicing cloud-based website hosting and deployment.

---

## Objective

The objectives of this project were:

* Understand Azure Blob Storage
* Create and configure an Azure Storage Account
* Enable static website hosting
* Upload website files to Azure Blob Storage
* Configure the website for public access
* Access the hosted website through the Azure static website endpoint
* Understand an alternative approach to VM-based website hosting

---

## Technologies Used

* Microsoft Azure
* Azure Storage Account
* Azure Blob Storage
* Static Website Hosting
* HTML/CSS Website Template
* Web Browser

---

## Architecture

```text
Website Template
       ↓
Azure Storage Account
       ↓
Blob Storage
       ↓
Static Website Hosting
       ↓
Static Website Endpoint
       ↓
Web Browser
```

Unlike the previous VM-based projects, this project does not require a virtual machine or a traditional web server such as Apache.

---

## Implementation Overview

### 1. Create a Storage Account

An Azure Storage Account was created to provide the storage infrastructure required for hosting the website.

### 2. Enable Static Website Hosting

The **Static Website** feature was enabled for the storage account.

This allows Azure Blob Storage to serve static website files through a web endpoint.

### 3. Upload Website Files

The website's static files were uploaded to the storage account.

These included files such as:

```text
index.html
CSS files
JavaScript files
Images and other assets
```

### 4. Configure the Website

The appropriate website entry file was configured so that Azure could serve the website when the static website endpoint was accessed.

### 5. Access the Website

After configuration and deployment, the generated Azure static website endpoint was opened in a web browser to verify that the website was accessible.

---

## Website

The website used in this project was a pre-existing template website.

The primary purpose of the project was to understand **cloud-based static website hosting using Azure Blob Storage**, rather than developing the website itself.

---

## Result

The website was successfully hosted using **Azure Blob Storage Static Website Hosting** and accessed through the generated static website endpoint.

### Screenshot

![Website hosted using Azure Blob Storage](./screenshot.png)

---

## Key Concepts Learned

* Azure Storage Accounts
* Azure Blob Storage
* Static website hosting
* Cloud-based website deployment
* Static website endpoints
* Storage-based hosting
* Difference between VM-based and serverless static website hosting

---

## Comparison with Previous Projects

This project provided an alternative to the VM-based hosting approaches used in the previous projects.

| Project   | Hosting Method                            |
| --------- | ----------------------------------------- |
| Project 3 | Windows Virtual Machine                   |
| Project 4 | Linux Virtual Machine + Apache            |
| Project 5 | Azure Blob Storage Static Website Hosting |

The Blob Storage approach eliminates the need to maintain a virtual machine or install a traditional web server for a purely static website.

---

## Limitations

The website used in this project was a template website and was not developed as a custom web application.

The original Azure storage environment used for the project is no longer available, so the repository contains the available final-result screenshot as evidence of the completed deployment.

---

## Future Improvements

Possible improvements include:

* Deploying a custom-built website
* Connecting a custom domain
* Configuring HTTPS
* Automating website deployment
* Integrating Azure CDN for improved content delivery
* Using CI/CD to automatically deploy website updates
* Adding monitoring and logging

