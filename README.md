# Ryzentosh B450x - RYZEN 5 5600G OPENCORE EFI
OpenCore EFI for B450 Gaming Plus Max Chipset + Ryzen 5 5600 APU with Radeon™ Integrated Graphics
> ### Advice
> - Generate your own SMBIOS, I recommend [OCAT](https://github.com/ic005k/OCAuxiliaryTools) which has a GUI or [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
> - Use MacBookPro16,3, iMac20,1 or iMacPro1,1 SMBIOS. I recommend using an iMac20,1.
MacPro7,1 might result in a black screen.

## Specs / Tested On 🖥️

- Motherboard : MSI B450 Gaming Plus Max
- BIOS : AMI VERSION 7B86vHK
- CPU : AMD Ryzen 5 5600G with Radeon Graphics
- RAM : 2 x 16GB DDR4 3200MHz
- iGPU : Radeon™ Vega 7 Integrated Graphics
- Ethernet : RTL8111H (Not Tested/Added)
- Audio : Realtek ALC897
- Boot Mode : UEFI
- Bootloader : OpenCore 1.0.4
- OS : macOS Ventura 13.5 & 14.7.4
- WIFI: Intel AX210 with FENVI PCI Adapter

## Working ✅
- CPU Power Management
- Shutdown and Restart
- Sleep
- All USB Ports
- WiFi
- HDMI
- Audio (Rear & Front)
- Bluetooth
- Etc

> [!TIP]
> - To make the pc sleep faster run this: 
>```sudo pmset dwlinterval 0```
> - Do **NOT** upgrade Bluetooth related Kexts or Bluetooth won't work and the PC will boot up slower.
>- Toggle **SetupVirtualMap** if you are stuck at `[EB|#LOG:EXITBS:START]`

## Not Working ❌
- iMessage and FaceTime (Can log in, but cannot communicate)
- Airdrop
- VDA Decoding
- DRM (use Chrome or Firefox for DRM)
## Not tested ℹ️
- Ethernet (kext not added, you can add [this](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#ethernet:~:text=instead-,RealtekRTL8111,with%20your%20Ethernet.%20If%20you%20see%20this%20issue%2C%20try%20older%20versions.,-LucyRTL8125Ethernet) kext for the B450 Gaming Plus Max mobo)
- HandOff
## Issues 
- Stated on [NootedRed FAQ](https://chefkissinc.github.io/applehax/nootedred/#:~:text=Chrome%2C%20Chromium%2Dbased,%2D%2Ddisable%2Dgpu): Chrome, Chromium-based browsers and apps like Sublime Text cause graphical artifacts amongst other problems.
- Sometimes drag and drop operations wont drop the file. To temporarily fix this just sleep and wake the pc.

## AMD BIOS Settings

### Disable
- Fast Boot
- Secure Boot
- Serial/COM Port
- Parallel Port
- Compatibility Support Module (CSM) (Must be off in most cases, GPU errors/stalls like gIO are common when this option is enabled)
- IOMMU


## Tutorial
- From Zero Tutorial : https://dortania.github.io/OpenCore-Install-Guide/
- Creating the USB Installer : https://dortania.github.io/OpenCore-Install-Guide/installer-guide/
- Generating SMBIOS : https://github.com/corpnewt/GenSMBIOS
- USB Fixes : https://dortania.github.io/OpenCore-Post-Install/usb/ and https://github.com/usbtoolbox/tool

Tutorial on "USB Fixes" related to the UTBMap.kext and SSDT-SLEEP.aml files. Please pay close attention to the guidelines that have been provided.

All kinds of errors and kernel panics, beyond my responsibility.


## Donating ❤️ (Not to me)
You can show your appreciation for this EFI by donating to the creator of NootedRed, [ChefKiss](https://github.com/ChefKissInc) to get Hardware Accelerated Chromium and DRM support for AMD IGPUs 😭🙏.

Donate to ChefKiss via [ko-fi](https://ko-fi.com/chefkiss) or Bitcoin at ```bc1qgu56kptepex2csuzl5nhzc4vxuj8c6ggjzhcem```

Thanks to Alfinauzikri for repo template: https://github.com/alfinauzikri/B550-5600G-6600XT-Hackintosh/blob/main/README.md?plain=1
# Screenshots
![2025-05-27_18 38 54](https://github.com/user-attachments/assets/b284dc62-9c32-4a00-b9c7-2546fc5d5c20)
![2025-05-27_18 40 55](https://github.com/user-attachments/assets/718df190-c4cb-4329-b2df-33641524fe40)


