# OpenCore-ASRock-B75-Pro3-M
OpenCore for OpenCore-ASRock-B75-Pro3-M with i5-3470

## OC information
* OC Version: 0.6.1
* Tested OS Version: 10.15.6, 11.0(Maybe?)(Failed in second install test)

## Test platform
* ASRock B75Pro3-M(Bios Version:2.0Beta)
* Intel I5 3470
* Kingston DDR3 8G * 2
* XFX RX470
* Intel AC3160

## Working
* CPU-PM(For i5-3470, if not, rebuild the SSDT-PM.aml)
* Sleep
* WLAN
* Bluetooth

## Before installation
### Edit config.plist
Using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate your own SMBIOS information(chose the MacPro6,1 SMBIOS) and write to config.plist

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

#### Enable
* SATA Mode: AHCI

## After installation
### Fixing iMessage and other services with OpenCore
[https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)

## Kext information
| Name                             | Version |
| -------------------------------- | ------- |
| Lilu                             | 1.4.7   |
| Innie                            | 1.2.1   |
| VirtualSMC                       | 1.1.6   |
| WhateverGreen                    | 1.4.2   |
| AppleALC                         | 1.5.2   |
| RealtekRTL8111                   | 2.3.0   |
| USBInjectAll                     | 0.7.5   |
| IntelBluetoothFirmware           | 1.1.2   |
| NVMeFix                          | 1.0.3   |
