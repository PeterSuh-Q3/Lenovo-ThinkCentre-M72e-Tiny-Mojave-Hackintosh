# Lenovo-ThinkCentre-M72e-Tiny-Mojave-Hackintosh
Lenovo ThinkCentre M72e Tiny Mojave Hackintosh, OpenCore 0.6.5

OpenCore 0.6.5 EFI folders for M72e i5 (HD2500) version (LAST BIOS F4KT61AUS 25-JUL-2018). 
Everything works fine.

In particular, this motherboard has a 6-series chipset, so I faked device-id 3A1E0000 for IMEI and add ACPI table SSDT-IMEI.
I followed this Manual. 
https://github.com/acidanthera/WhateverGreen/blob/master/Manual/FAQ.IntelHD.en.md

M72e has a bug that does not recognize OpenCore Bootx64.efi in the BIOS. So, instead, I had to rename as SUSE's elilo.efi file.

Since it succeeded in similar tiny specifications, it will be available in Small and Tower.


## System Specs

| Part | Model Number
| --- | ---
| CPU | Intel(R) Core(TM) i5-3470T CPU @ (2.90GHz, 3MB Cache)
| Chipset | Intel H61 Express Chipset
| iGPU | Intel HD Graphics 2500
| Storage | Samsung 840EVO SSD 120GB
| Memory | Samsung 4GB 2Rx8 PC3 - 12800S (DDR3 1600MHz) x 2EA (PN: M471B5273DH0-CK0)
| Audio | Realtek ALC662
| Ethernet | Realtek RTL8111E
| Wi-Fi | Intel(R) Centrino(R) Advanced-N 6235 AGN
| OpenCore | 0.6.5
| SMBIOS | iMac13,2
