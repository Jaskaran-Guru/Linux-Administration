Experiment 3 --> Installation and Configuration: Preparing for installation (hardware requirements, partitioning with Gparted)

Installation and Configuration of Linux

Installing Linux requires preparing the system by checking hardware compatibility, creating bootable media, and setting up partitions.

1. Preparing for Installation

A. Hardware Requirements

Different Linux distributions have varying system requirements. Below are the general requirements:

Component	Minimum Requirements	Recommended Requirements
Processor	1 GHz (x86_64 or ARM)	2 GHz dual-core or better
RAM	1 GB (for lightweight distros like Lubuntu)	4 GB or more
Storage	10 GB	25 GB or more
Graphics	Integrated GPU	Dedicated GPU (for gaming or design)
Internet	Not mandatory	Recommended for updates
For lightweight systems, Xubuntu, Lubuntu, and Puppy Linux work well on older hardware.

B. Creating Bootable Media

Before installation, you need to create a bootable USB/DVD.

Steps to Create a Bootable USB

Download ISO File:

Get the official Linux ISO from the distribution’s website (e.g., Ubuntu, Debian).
Use a Bootable USB Creator:

Rufus (Windows)
Etcher (Windows, Mac, Linux)
dd command (Linux terminal)
Boot from USB:

Restart the computer and enter BIOS/UEFI settings (Press F2, F12, Del, or Esc).

Select USB drive as the boot device.

2. Partitioning with GParted

GParted (GNOME Partition Editor) is a tool for managing disk partitions before installing Linux.

A. Why Partition?

Partitioning separates system files from user data and improves system performance.

B. Recommended Partitions for Linux

Partition	Type	Size	Description
Root (/)	Ext4	20 GB or more	Stores the OS and system files
Swap	Swap	Equal to RAM (if RAM < 8GB)	Used as virtual memory
Home (/home)	Ext4	Remaining space	Stores user data and settings
EFI (/boot/efi for UEFI systems)	FAT32	100-500 MB	Needed for UEFI boot

C. Steps to Partition Using GParted

Boot into Live USB (Try Ubuntu before installation).
Open GParted (sudo gparted).
Select Your Hard Drive (e.g., /dev/sda).
Create Partitions (Use the recommended sizes).
Apply Changes and close GParted.
Proceed with Linux installation and assign partitions accordingly.
