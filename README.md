# OpenCore-ASRock-B450-Gaming-ITX-ac
OpenCore for ASRock B450 Gaming-ITX/ac

## OC information
* OC Version: 0.5.9

## Test platform
* ASRock B450 Gaming-ITX/ac
* AMD Ryzen R5 3600
* CUSO DDR4 2666 16G * 2
* XFX RX470

## Working
* WIFI (*Modify `EFI/OC/Kexts/itlwm.kext/Contents/Info.plist` to set your WiFi SSID and password.*)
* Bluetooth

## Known issues
No Mic on AMD:
* This is a common issue with when running AppleALC with AMD, specifically no patches have been made to support Mic input. At the moment the "best" solution is to either buy a USB DAC/Mic or go the VoodooHDA.kext method. Problem with VoodooHDA is that it's been known to be unstable and have worse audio quality than AppleALC

## Before installation
### BIOS Settings
### Disable

* Fast Boot
* Secure Boot
* Compatibility Support Module (CSM)
* Above 4G decoding

## After installation
### Fixing iMessage and other services with OpenCore
[https://dortania.github.io/OpenCore-Desktop-Guide/post-install/iservices.html](https://dortania.github.io/OpenCore-Desktop-Guide/post-install/iservices.html)

### Enable trim
`sudo trimforce enable`

## Credits
[zxystd/itlwm](https://github.com/zxystd/itlwm)
[zxystd/IntelBluetoothFirmware](https://github.com/zxystd/IntelBluetoothFirmware)