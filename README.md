# OpenCore-B75Pro3M-i5-3470
OpenCore for B75Pro3-M i5-3470

## OC information
* OC Version: 0.6.1
* Tested OS Version: 11.0 Beta3, 10.15.6

## Test platform
* ASRock B75Pro3-M(Bios Version:2.0Beta)
* Intel I5 3470
* Kingston DDR3 8G * 4
* XFX RX470

## Working
* CPU-PM
* Sleep

## Before installation
### Edit config.plist
Using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate your own SMBIOS information(chose the MacPro7,1 SMBIOS) and write to config.plist

* The Type part gets copied to Generic -> SystemProductName.

* The Serial part gets copied to Generic -> SystemSerialNumber.

* The Board Serial part gets copied to Generic -> MLB.

* The SmUUID part gets copied to Generic -> SystemUUID.

### BIOS Settings
#### Disable
* Fast Boot
* Secure Boot
* Serial/COM Port
* Parallel Port
* CSM
* Thunderbolt(For initial install, as Thunderbolt can cause issues if not setup correctly)
* Intel SGX
* Intel Platform Trust

#### Enable
* CFG Lock
* VT-d
* Above 4G decoding
* Hyper-Threading
* Execute Disable Bit
* EHCI/XHCI Hand-off
* OS type: Windows 8.1/10 UEFI Mode
* SATA Mode: AHCI

## After installation
### Fixing iMessage and other services with OpenCore
[https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)

## Kext information
| Name                             | Version |
| -------------------------------- | ------- |
| Lilu                             | 1.4.7   |
| VirtualSMC                       | 1.1.6   |
| WhateverGreen                    | 1.4.2   |
| AppleALC                         | 1.5.2   |
| RealtekRTL8111                   | 2.3.0   |
| USBInjectAll                     | 0.7.5   |
| MacProMemoryNotificationDisabler | 1.1     |
