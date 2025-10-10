# Implementing LASI's Intel 82596 NIC and NCR710 SCSI Controller for the PA-RISC Machines in QEMU


# Project Goal
- Implement a working device model for the Intel 82596 in QEMU.
- Implement a working device model for the NCR710 SCSI Controller in QEMU




# Work Report

82596 Network Interface Card
----------------------------
[x] Monitor Mode
[x] Timer
[x] Bus Throttle
[x] Promiscious Mode
[x] Get 82596 Working on HPUX
[x] Self test
[x] Accurate CU and RU transition State
[x] Reset Values
[x] Linear Segmented and 82596
[x] Support for Little endian mode
[x] VMstate descriptors
[x] Polling mechanism

What is still left:
[-] RX and TX function (Note: RX and TX function is working for Linux, but not for HPUX 10.20)
[-] Statistical counters (Paritially implemented)


PRs:


NCR710 SCSI Controller
----------------------
[x] Design from ground up
[x] Compatibiality testing as PCI Device from the WinUAE
[x] Implementation with Seabios
[x] Adding LASI_NCR710 support to QEMU
[x] Redesigned the NCR710 entirely from the linux kernel

PRs:

Final Result: Working NCR710 SCSI Controller for linux



Future Work
-----------
- Add NCR710 Support for the HPUX 10.20: 
This requires minimal work considering but have to iron out a few changes, it seems that the HPUX is currently facing kernel panic. I have added proper trace functions so it would be easier for me to debug the NCR710 and add HPUX 10.20 support.
