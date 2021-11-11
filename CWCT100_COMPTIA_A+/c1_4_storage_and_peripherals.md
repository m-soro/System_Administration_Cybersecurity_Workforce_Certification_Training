---
layout: default
title: Core 1 - 4 Storage and Peripherals
parent:  CWCT CompTIA A+
nav_order: 4
---




# Storage and Peripherals

## 1. Mass Storage Technologies

### Introduction to mass storage
> Given a scenario, select, install and configure storage devices

* **Logical Block Addressing(LBA)** - all storage have this
* Capacity - how many blocks in storage

Two different ways of counting blocks:

In Decimal:
* **1,000 = Kilo**
* **1,000,000 = Mega**
* **1,000,000,000 = Giga**
* **1,000,000,000,000 = Tera**
* **1,000,000,000,000,000 = Peta**
*  **1,000,000,000,000,000,000 = Exa**

In IEC:
* **2^10 = Kibi**
* **2^20 = Mebi**
* **2^30 = Gibi**
* **2^40 = Tebi**
* **2^50 = Pebi**
* **2^60 = Exbi**

#### Quick Review
* There are many types of mass storage used today, including hard drives, solid state drives and optical media
* Regardless of the media your operating system sees, mass storage as a string of logical bloack addresses
* There is a difference between decimal values and IEC values

### Magnetic disk drives
![Screen Shot 2021-11-03 at 6 03 19 AM](https://user-images.githubusercontent.com/63247801/140041045-2996c93a-f9a9-452d-9de9-64cb6d70045f.png)

**Hard disk drive** - has something spinning inside, sizes are: 3 1/2 and 2 1/2.

**How to speak with disk drives?**

* It uses **Advanced Technology Attachment(ATA)**, has been around since 1990, however the physical interface change which is **Parallel ata(PATA)** which is long dead and not on the exam.

* What we see today is **Serial ATA(SATA)**

![Screen Shot 2021-11-03 at 6 08 38 AM](https://user-images.githubusercontent.com/63247801/140041802-3dc639d2-e297-46f0-b700-01e1981673bb.png)

>power

![Screen Shot 2021-11-03 at 6 09 46 AM](https://user-images.githubusercontent.com/63247801/140041965-e0142177-705b-4d3e-b481-d8a5849fd62a.png)

>SATA cable

* All motherboards has SATA built in
* drives need SATA connection(for data) and sata power cable, then thats it

* **ESATA** - designed to be used EXternally **Its in A+ exam**
* There is also ESATA expansion card

#### Quick Review
* Magnetic disk drives use spinning platters to store data via magnetism and read/write heads
* Hard disk drives come in 3.5, 2.5, and 1.8 physical sizes
* We use the AT attachment protocol to communicate with hard disk drives
* The dominan ATA is called Serial ATA(ATA)

### Solid State Drives(SSD)
* faster, used primarily as boot system
* 2 1/2 in is most common

this is an m.2 SSD - this sizes are most common
![Screen Shot 2021-11-03 at 6 20 15 AM](https://user-images.githubusercontent.com/63247801/140043471-ba759d8b-d689-4117-bec6-3512f0874069.png)

* SSD is Fast, the traditional SATA interface is not fast enough for SSD.
* It uses **Non-Volatile Memory Express(NVME)** much faster than SATA, becoming more common
* Makes sure motherboard is correct inteface for SSD

#### Quick Review
* Solid state drives (SSDs) store data using chips; there are no moving parts
* Data is stored in blocks and pages
* SSDs come in traditional 3.5" and 2.5" sizes, but also come in M.2 format
* Some SSDs use the very fast NVMe protocol instead of ATA for increased performance

### Small Computer System Interface (SCSI)

![Screen Shot 2021-11-03 at 6 31 11 AM](https://user-images.githubusercontent.com/63247801/140044997-9cfdc8ad-8ba3-4937-8903-6602b630f401.png)

![Screen Shot 2021-11-03 at 6 31 41 AM](https://user-images.githubusercontent.com/63247801/140045062-8e663749-a03a-49af-9274-d6eba92bd6e5.png)
Its about 25 years old, developed same time as ATA, compatible with each other

**These two types are dead**

**Serial Attached SCSI** looks like SATA but not compatible, used in server
![Screen Shot 2021-11-03 at 6 33 18 AM](https://user-images.githubusercontent.com/63247801/140045267-0c07d4fc-ab0d-4bc1-8f33-dc5aeb3b4a29.png)

ISCI - has SCSI connection but in a network

#### Quick Review
* The Small Computer Systems Interface (SCSI) is an ancient standard that still has great support
* The old parallel SCSI is standard, but the SCSI lanfuage lives on in serial SCSI versions
* Two modern SCSI standards are SAS(Serial Attached SCSI), iSCSI

### Boot Order

When you have a lot of storage, you have to define the boot order

#### Quick Review
* When a system boots, it looks for a bootable devices
* Its important to make sure the system looks for the correct boot devices
* The boot order is defined in the system setup


### 2. Implementing Mass Storage

**Just a bunch of disk(JBOD)**

**Redundant array of independent disks(RAID)** - speed and data redundancy

* **RAID 0 or Striping** - speed but not data safety. half & half of data
* **RAID 1 or Mirroring** - redundant data, slower
* **RAID 5 or Parity** - minimum of three drive, good speed and redundacy of data, can lose only one drive
* **RAID 6** - requires min of four drives(more popular than RAID 5), can lose 2 drives
* **RAID 10 or Striping Mirrors** - Striping two mirrored pairs, you can lose one mirrored pair in each side, but not paired mirrors
* **RAID 01** - zero plus one, two stripes and mirror them

#### Quick Review
* RAID provides speed and/or redundacy
* RAID 0 (striping) provides speed
* RAID 1 (mirroring) provides redundancy
* RAID 5 and 6 (striping with parity) provides speed and redundancy
* RAID 5 can only lose one drive in the array; RAID 6 can lose two

### Hardware RAID
Means we have controllers that talks to hard drive that configures hard drive

Hot spare - if hard drive fails, it jumps and re build the array
hotswappable - means you dont have to turn off the computer

#### Quick Review
* Hardware RAID requires a controller to configure the RAID arrays
* Hardware RAID has its own BIOS that comes with a special system setup to configure the RAID array
* The completed array looks like a single drive to the operating system

### Mass storage troubleshooting - Objective 5.3
> Given a scenario, troubleshoot hard drives and RAID arrays

1. Back it up
2. Mental Reinstall
3. Triple Check

RAID not found/ RAID not working
RAID stopped working
Read/Write Failure
Slow Performance
Loud clicking
Failure to boot
Drive not recognized
OS Not Found
Attemps to boot to incorrect device
Continuos Reboot

S.M.A.R.T. - if a drive starts to act up

#### Quick Review
* Always back up important data before troubleshooting mass storage
* Use mental process of installaation to make sure all the installation steps have taken place
* Review the many symptoms in this episode!

### 3. Essential Peripherals

### Optical Media

#### Quick Review
* Compact discs (CDs) store 650-700 MB of data
* Digital video discs (DVDs) store from 4.37 GB to 15.9 GB
* Blue-rays store from 15.6 GB to 50 GB capacity

![Screen Shot 2021-11-10 at 6 35 05 AM](https://user-images.githubusercontent.com/63247801/141106063-b0fe41c6-a8f7-476f-848f-173cc1afb34e.png)

* All optical media comes in read only (ROM), write once (R) and write many (RW) versions

### Universal Serial Bus (USB)

* For exam, make sure you know USB speeds
* 
![Screen Shot 2021-11-11 at 5 49 17 AM](https://user-images.githubusercontent.com/63247801/141285452-28c7d772-2dda-4fb8-ade3-37019bd3ab27.png)



* Recognize the connectors

#### Quick Review

* Universal Serial Bus (USB) 1.1 comes in 1.5 MB/s and 12 Mbps; USB 2.0 runs at 480 Mbps
* USB 3.0 runs at Gbps; USB 3.1 runs at 10 Gbps
* USB versions often use colors to show version
* USB connectors come in many types: Type-A, Type-B, Type-C, standard, mini and micro.

### Understanding USB

**USB Controller**

![Screen Shot 2021-11-11 at 5 52 27 AM](https://user-images.githubusercontent.com/63247801/141285856-756e4e77-640e-4aa1-b9c7-beeddab823c4.png)

![Screen Shot 2021-11-10 at 6 36 00 AM](https://user-images.githubusercontent.com/63247801/141106184-9b47a35d-9bd7-4c5c-b19a-e8a0f8434d13.png)

#### Quick Review
* All USB devices connect to the USB controllers built into the motherboard of the system; the USB controller is in charge of all connected USB devices
* This creates an upstream/downstream concept
* USB Type-A connectors connect downstream USB Type-B connectors connect upstream, though there are exceptions

### Configuring USB

* **Human Interface Devices(HID)** makes keyboard and mice work, base driver
* **Disable USB Port**
* **USB Lock**

#### Quick Review
* USB devices must have a device driver
* Operating systems come with thousands of built-in device drivers
* In some cases, you may need to download the correct driver for a USB device from the Internet

### Thunder and Lightning

Thunderbolt kind of a mix of PCIe and display: 

![Screen Shot 2021-11-11 at 6 05 37 AM](https://user-images.githubusercontent.com/63247801/141287666-40422749-0c31-4f53-91ee-50f73518d4a2.png)
![Screen Shot 2021-11-11 at 6 06 16 AM](https://user-images.githubusercontent.com/63247801/141287758-089b0e7e-5f95-48fe-bc18-c66a0b77b675.png)
![Screen Shot 2021-11-11 at 6 06 30 AM](https://user-images.githubusercontent.com/63247801/141287801-0af32eda-059f-4044-8c8d-cc0d620f0c0c.png)

Lightning - exclusive to Apple

Charging and data transfer, slower than Thuderbolt

#### Quick Review
* Thuderbolt is a general purpose I/O port that runs at 10Gbps up to 40 Gbps
* Thunderbolt uses a mini DisplayPort or a USB C connector
* The Lightning standard is exlusive to Apple products
* Lightning uses a proprietary lightning connector

### Keyboard and Mice

#### Quick Review
* Keyboards use either a USB or PS/2 connection
* Mice almost exclusively use USB
* Game controllers often have a proprietary connection that requires a converter piece
* Keyboard Video Mouse (KVM) switches give the ability for a single keyboard, monitor and mouse to connect multiple computers

### Sight and Sound

![Screen Shot 2021-11-11 at 6 20 44 AM](https://user-images.githubusercontent.com/63247801/141289915-1791182a-873a-4e19-9a0c-e8831c3184d1.png)
![Screen Shot 2021-11-11 at 6 24 15 AM](https://user-images.githubusercontent.com/63247801/141290008-d0467d6f-7b68-4c93-baab-fd09b29c9826.png)

#### Quick Review
* Sound is commonly built into todays systems
* Speaker systmes come into combinations with name like 2.1 or 5.1 systems.
* Sound uses 3.5 mm jacks or SPDIF
* Many devices like web cams or headsets, include speakers

### Readers and Scanners

![Screen Shot 2021-11-11 at 6 30 47 AM](https://user-images.githubusercontent.com/63247801/141290894-88fab9f1-2c8a-4abf-9a34-5b3a2313629a.png)
Automated Document Feeder(ADF)
Barcode/QR Code Scanners

#### Quick Review

* Smart cards/Magnetic readers are used to read cards
* Flash memory readers read many types of flash memory
* SD Cards are very popular flash memory
* Scanners read paper documents. Automatic document feeders enable multiple pages to scan
* Barcode and QR code scanners read printed coded labels

### Using expansion cards

#### Quick Review

* Always handle expansion cards carefully, avoiding the contacts
* Apply power, data connections or dongles as needed
* Make sure to add the correct driver, check Device Manager to confirm good drivers
* A new device installation is a common place for Blue Screen of Death screens
