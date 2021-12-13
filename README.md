# Lenovo-ThinkCentre-M72e-Tiny-Mojave-Hackintosh

![스크린샷 2021-12-13 오전 10 49 16](https://user-images.githubusercontent.com/85427533/145748236-ee839a38-5025-45a6-8696-f7f6b95d3e7d.png)

OpenCore 0.6.5 EFI folders for M72e i5 (HD2500) version (LAST BIOS F4KT61AUS 25-JUL-2018). 
Everything works fine.
![211211_lec_7cba046656568a050501e26efc1fcf45ec59330c](https://user-images.githubusercontent.com/85427533/145748417-6c89b8f5-bfd9-4d2c-b23f-fa15f5de3941.png)

In particular, this motherboard has a 6-series chipset, so I faked device-id 3A1E0000 for IMEI and add ACPI table SSDT-IMEI.
I followed this Manual. 
https://github.com/acidanthera/WhateverGreen/blob/master/Manual/FAQ.IntelHD.en.md

M72e has a bug that does not recognize OpenCore Bootx64.efi in the BIOS. So, instead, I had to rename as SUSE's elilo.efi file.

Since it succeeded in similar tiny specifications, it will be available in Small and Tower.



[BIOS SETUP]

1.SATA AHCI activation. (Don't touch the AHCI part as the default, just check it.)



2. Switch to UEFI Only mode.

![211210_lec_2e2da54d2450d760799a9d7cd07c4f608e0f658d](https://user-images.githubusercontent.com/85427533/145748980-d2c6c48c-ad49-4c16-93b6-14e5a3b71b50.jpeg)
![211210_lec_f7a4b0fa9e9c2eeba3ca1ae4311bfc9bf8f14acd](https://user-images.githubusercontent.com/85427533/145748446-96acc331-7dcb-474e-965b-7fd817e8661d.jpeg)



3. Secure Boot Mode, disable change (disable to secure boot mode )

![211210_lec_db26f0770524cff0aa252981bff40c92eee617dc](https://user-images.githubusercontent.com/85427533/145748501-e58e8042-a0ee-4b48-afb5-3b9323e9986f.jpeg)
![211210_lec_b61bb1d9f5672003586b5b882751c60bdd3dc881](https://user-images.githubusercontent.com/85427533/145748517-5abef6ca-34bb-4a7d-b767-071f5501a00b.jpeg)


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
| MAC OS | 10.14.06 Mojave


