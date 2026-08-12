# Mounting Azure File Share on Windows VM

## Overview

This project demonstrates how to create and access an **Azure File Share from a Windows Virtual Machine**.

The Azure File Share was used to store website-related files, including HTML, CSS, JavaScript, and image files. The file share was then mounted on a Windows VM so that the files could be accessed from the virtual machine.

This project helped me understand how cloud-based file storage can be integrated with virtual machines.

---

## Objective

The main objectives of this project were:

* Understand Azure Files and Azure File Shares
* Create and manage a file share in an Azure Storage Account
* Upload files to an Azure File Share
* Mount the Azure File Share on a Windows Virtual Machine
* Access cloud-stored files from a Windows VM
* Understand the relationship between cloud storage and virtual machines

---

## Technologies Used

* Microsoft Azure
* Azure Storage Account
* Azure File Share
* Windows Virtual Machine
* SMB File Sharing
* HTML
* CSS
* JavaScript

---

## Architecture

```text
Website Files
     │
     ▼
Azure Storage Account
     │
     ▼
Azure File Share
     │
     │  SMB
     ▼
Windows Virtual Machine
     │
     ▼
Access / Manage Files
```

---

## Implementation Overview

### 1. Create an Azure Storage Account

An Azure Storage Account was used as the storage service for the project.

### 2. Create an Azure File Share

A file share named `websitehosting` was created inside the storage account.

The file share was used to store the website files.

The stored files included resources such as:

```text
index.html
CSS files
JavaScript files
Images
Other website assets
```

### 3. Upload Website Files

The website files were uploaded to the Azure File Share.

The Azure portal was used to browse and manage the files stored in the share.

### 4. Mount the File Share on Windows VM

The Azure File Share was mounted on a Windows Virtual Machine.

This allowed the Windows VM to access the files stored in Azure Files as a remote file share.

### 5. Access the Files

After mounting the share, the files stored in Azure could be accessed from the Windows VM.

This demonstrated how centralized cloud storage can be connected to a virtual machine for file access.

---

## Azure File Share Contents

The file share contained website-related files, including:

```text
images/
index.html
templ...-script.js
templ...-style.css
timer.html
```

The exact files depended on the website template used for the demonstration.

---

## Result

The Azure File Share was successfully accessed from the Windows Virtual Machine.

The Azure portal showed the `websitehosting` file share and its stored website files, demonstrating that the files were available through Azure Files.

## Key Concepts Learned

* Azure Storage Accounts
* Azure Files
* Azure File Shares
* Cloud-based file storage
* Windows Virtual Machines
* SMB-based file sharing
* Mounting remote file shares
* Accessing cloud storage from a VM
* Separation of compute and storage

---

## Why Azure Files?

Azure Files allows files to be stored separately from the virtual machine while still making them accessible from supported systems.

This provides a useful separation between:

```text
Compute → Windows Virtual Machine

Storage → Azure File Share
```

This means that files can be stored in Azure Files without requiring them to be stored directly on the VM's local disk.

---

## Project Significance

This project demonstrates an important cloud-computing concept: **separating storage from compute**.

Instead of keeping all files directly on the Windows VM, the files were stored in Azure File Share and accessed from the VM when required.

This approach can be useful when multiple systems or applications need access to shared files.

---

## Limitations

This was a hands-on learning project using a website template and was primarily focused on understanding Azure File Share integration with a Windows VM.

The original VM and storage environment used for the demonstration may no longer be available. The repository therefore contains the available screenshot as evidence of the completed setup.

---

## Future Improvements

Possible improvements include:

* Mounting the same Azure File Share on multiple virtual machines
* Using Azure Files for shared application storage
* Configuring persistent access to the file share
* Implementing access control and secure authentication
* Integrating the file share with applications running on Azure VMs
* Exploring Azure File Sync
