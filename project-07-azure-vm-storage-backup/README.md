# Azure VM Storage, Snapshot & Backup

## Overview

This project demonstrates practical management of **storage, disks, snapshots, and backup for an Azure Virtual Machine**.

The project involved attaching a data disk to a Windows VM, verifying the disk from within the Windows operating system, creating an Azure managed-disk snapshot, and configuring Azure VM Backup with recovery points.

The project provided hands-on experience with protecting and extending VM storage in Azure.

---

## Objectives

The main objectives of this project were:

* Understand Azure VM disk management
* Attach an additional data disk to a virtual machine
* Verify the attached disk from Windows
* Understand Azure managed disks
* Create a snapshot of a VM disk
* Configure Azure VM Backup
* Understand recovery points and VM data protection

---

## Technologies & Services Used

* Microsoft Azure
* Azure Virtual Machine
* Azure Managed Disks
* Azure Disk Snapshot
* Azure Backup
* Recovery Services Vault
* Windows
* DiskPart

---

## Architecture

```text
                 Azure Virtual Machine
                         │
             ┌───────────┴───────────┐
             │                       │
          OS Disk                Data Disk
          127 GiB                 1 TiB
             │                       │
             │                       ▼
             │                 Windows VM
             │                       │
             ▼                       ▼
        VM Snapshot              Data Storage
             │
             ▼
      Azure Backup
             │
             ▼
    Recovery Point / Vault
```

---

## Implementation Overview

### 1. Attach a Data Disk

An additional **1 TiB data disk** was attached to the Windows virtual machine.

The Azure VM disk configuration showed the additional disk attached as a data disk.

---

### 2. Verify the Disk in Windows

The Windows VM was used to verify the available disks using the Windows command-line `DiskPart` utility.

The `list disk` command displayed the available disks and their sizes.

Example:

```text
DISKPART> list disk
```

This provided practical experience in identifying disks from inside the operating system.

---

### 3. Verify VM Disk Configuration

The Azure portal was used to inspect the VM's disk configuration.

The VM had:

* An OS disk
* An additional data disk
* Configured storage performance settings

This demonstrated how Azure VMs can use separate disks for operating-system and application/data storage.

---

### 4. Create a Disk Snapshot

A snapshot named `snap` was created for the VM's OS disk.

The snapshot information showed:

* Snapshot type: Incremental
* VM generation: Gen 2
* Provisioning state: Succeeded
* Size: 127 GiB
* Storage type: Zone-redundant

A disk snapshot provides a point-in-time copy that can be used as part of a recovery or disk-management workflow.

---

### 5. Configure Azure VM Backup

Azure VM Backup was configured using a **Recovery Services vault**.

The backup configuration showed:

* Backup pre-check: Passed
* Last backup status: Successful
* Recovery points available
* Included disks: All disks

This demonstrated how Azure Backup can be used to protect a virtual machine.

## Key Concepts Learned

* Azure Managed Disks
* OS disks and data disks
* Attaching data disks to VMs
* Disk management in Windows
* DiskPart
* Azure disk snapshots
* Incremental snapshots
* Azure Backup
* Recovery Services Vault
* Recovery points
* VM data protection

---

## Project Significance

This project demonstrates that VM management involves more than simply creating and running a virtual machine.

Storage management and backup are important parts of maintaining a reliable cloud environment. The project provided hands-on experience with both **additional VM storage** and **data protection mechanisms** in Azure.

---

## Future Improvements

Possible improvements include:

* Creating and restoring a VM from a snapshot
* Formatting and partitioning the data disk
* Moving application data to the data disk
* Testing a complete VM restoration
* Exploring backup retention policies
* Testing recovery from a selected recovery point
* Monitoring disk performance
