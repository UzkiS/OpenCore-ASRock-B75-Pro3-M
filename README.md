# OpenCore-ASRock-B75-Pro3-M
OpenCore for OpenCore-ASRock-B75-Pro3-M with G1610

## OC information
* OC Version: 0.6.2
* Tested OS Version: 10.15.7

## Test platform
* ASRock B75Pro3-M(Bios Version:2.0Beta)
* Intel Celeron G1610
* Kingston DDR3 8G
* Dataland HD7850 1G D5

## Working
* CPU-PM(For G1610, if not, [rebuild the SSDT-PM.aml](https://dortania.github.io/OpenCore-Post-Install/universal/pm.html#sandy-and-ivy-bridge-power-management))
* Sleep

## Before installation
### Edit config.plist
Using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate your own SMBIOS information(chose the iMac20,2 SMBIOS) and write to config.plist

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
* CSM(unnecessary)

#### Enable
* SATA Mode: AHCI

## After installation
### Fixing iMessage and other services with OpenCore
[https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)

## Kext information
| Name                             | Version |
| -------------------------------- | ------- |
| Lilu                             | 1.4.8   |
| Innie                            | 1.2.1   |
| VirtualSMC                       | 1.1.7   |
| WhateverGreen                    | 1.4.3   |
| AppleALC                         | 1.5.3   |
| RealtekRTL8111                   | 2.3.0   |
| USBInjectAll                     | 0.7.5   |
| NVMeFix                          | 1.0.4   |
