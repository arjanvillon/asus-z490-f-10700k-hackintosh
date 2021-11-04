# Asus ROG Strix Z490-F Hackintosh

This repository is a hackintosh following the [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) using OpenCore 0.7.4. The MacOS version is 11.5. If you have a similar hardware, feel free to use my EFI and change the config on the [PlatormInfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo) section of the config.plist.

## Hardware

| Device      | Model                                        |
| ----------- | -------------------------------------------- |
| CPU         | Intel Core i7-10700k                         |
| Motherboard | Asus ROG Strix Z490-F                        |
| RAM         | Corsair Vengeance LPX 3000Mhz 16gb (8gb x 2) |
| ROM         | ADATA XPG SX8200 Pro 500gb                   |
| GPU         | HIS RX 580 8gb                               |
| Network     | Intel I225-V                                 |
| Case        | Corsair 4000D Airflow                        |

## BIOS settings

Some of my settings are a bit different from OpenCore's recommended settings. But please do check out their documentation

### Disable
- Fast Boot
- Serial/COM port
- Intel SGX

### Enable
- VT-d
- VT-x
- CSM
- Above 4G decoding
- EHCI/XHCI hand-off

### Other Settings
- Secure Boot: set OS type to Other OS
- CFG lock: no such option, already unlocked

## Working
- [x] CPU/Motherboard
- [x] iGPU (I set my config to not use it as display)
- [x] GPU
- [x] Audio
- [x] Intel i225-V Ethernet (by adding a boot arg on the config)
- [x] Bluetooth (I use a dongle so I didn't had to add any kexts for it)
- [x] Shutdown / Restart
- [x] Sleep / Wake
- [x] USB Ports
- [x] Power Management

## Theme
I use [BsxM1](https://github.com/blackosx/BsxM1) which is really awesome. But feel free to change the theming based on your taste by following [Dortania's Cosmetics Guide](https://dortania.github.io/OpenCore-Post-Install/cosmetic/gui.html#setting-up-opencore-s-gui).