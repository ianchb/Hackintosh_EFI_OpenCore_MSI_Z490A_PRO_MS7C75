# Hackintosh_EFI_OpenCore_MSI_Z490A_PRO_MS7C75
EFI(based on OpenCore without GUI) files for MSI Z490A-PRO(MS7C75). Intel UHD graphics is NOT tested.  
also available at https://cgtsoft.com/archives/108/.
## Before we start...
**I am not responsible for your PC. For example, if your mishandling causes your PC to ~~become a tree and~~ not boot, you are responsible for it.**  
## Some of my hardware
|Hardware|Detail|
|  ----  | ----  |
|Motherboard|MSI Z490-A PRO (MS-7C75)|
|CPU|Intel i5-10600KF|
|Memory|ADATA XPG-Z1 DDR4-3600 8G*2|
|Graphic|GIGABYTE Radeon RX 5500 XT|
|SSD|WD_BLACK SN750 500GB|
|Wi-Fi & Bluetooth|BCM94360CD|
## Supported macOS versions
- [x] 10.15 Catalina  
- [x] 11 Big Sur  
- [x] 12 Monterey  
- [x] 13 (Beta 4) Ventura  
## OK, Let's start. How to use it?
- Download latest EFI files (**EFI_ms7c75_xxx.zip**) from [**Releases**](https://github.com/ianchb/Hackintosh_EFI_OpenCore_MSI_Z490A_PRO_MS7C75/releases) and unzip it. Please note that there may be Pre-release versions which can be unstable but includes new features.  
![image](https://user-images.githubusercontent.com/45872450/175772521-2c06b751-26c3-44cd-950e-1591f369b654.png)
- Customize your USBPorts.kext. You can get the template from **USB.zip**.  
Just delete the unneeded ports according to the callout (JUSBx) next to the USB ports in use on the motherboard.  
Customization is finished when 15 ports remain. (JUSB3/4 need additional confirmation)  
Guide: https://cgtsoft.com/archives/203/  
![image](https://user-images.githubusercontent.com/45872450/175773594-0f82b192-b324-4ec6-bba1-287b1d1436cd.png)
- Replace your custom USBPorts.kext in ..\OC\Kexts. Then put all files into ESP (EFI System Partition) and add Opencore.efi to the boot menu.
- Check your BIOS settings. Here's something you care:  
Based on **7C75v2D**. Download BIOS from [MSI](https://download.msi.com/bos_exe/mb/7C75v2D.zip).  
![image](https://user-images.githubusercontent.com/45872450/175774548-ff5365da-f6b5-47db-adb7-1af147efb070.png)  
**Enable VT-d**  
**Enable Resizable BAR**  
**Disable CFG Lock**
- Enjoy!  
![image](https://user-images.githubusercontent.com/45872450/175775443-bc20a2ed-c645-4844-82ba-1ba91869480e.png)
