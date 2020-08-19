# Hackintosh-HP-Z420-OpenCore
### Do not just copy this EFI and expect it to work
Hackintosh EFI for HP Z420 Workstation Using Catalina/Big Sur Beta   
# Setup
This EFI is setup for debugging, it uses the debug version of OpenCore, and has logging/verbose enabled.   
### Required BIOS Settings
Version 3.96 (Latest)    
SATA Mode - AHCI   
Enable Legacy ACPI CPU Tables   
### Create USB Installer
https://dortania.github.io/OpenCore-Install-Guide/installer-guide/ - Follow this guide to add macOS to the USB.   
Mount the EFI Partition.   
Copy the EFI files from the release zip file into your EFI partition.    
You will need to generate a MacPro6,1 SMBIOS using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS).  
You may have to edit the SSDT-GPU-SPOOF.aml if you have a different GPU. (You can most likely remove this if you have a fully supported GPU)   
Follow [This Guide](https://dortania.github.io/Getting-Started-With-ACPI/Universal/spoof.html) to edit it. Do not change the Device ID, but you need to change the Model and PCIe Root. (Explained in the guide)  
Boot the USB installer and install macOS.  
### Post Install
https://dortania.github.io/OpenCore-Post-Install/ - Steps are outlined in this guide.   
Mount your drives EFI partition and copy the contents of your USB installer's EFI partition to your drives EFI Partition.   
Convert fron the debug version of opencore to the release version, cleanup logging etc. Follow [This Guide](https://dortania.github.io/OpenCore-Post-Install/cosmetic/verbose.html#macos-decluttering).   
Follow any other steps you would like to complete your hackintosh.    
# My System
Intel Xeon E5-1650 v2 CPU  
Nvidia Quadro K4000 GPU   
32GB ECC DDR3   
# Issues
USB3 - The Z420 uses a Texas Instruments USB 3 Controller which is unsupported in MacOS   
DRM - My GPU is incompatable so DRM will never work for me   
Proper Audio(AppleALC)/Internal Speaker. (Workaround is to use VooDooHDA)   
Sleep doesn't work - you need to disable it inside of macOS.  
If you have any other issues, feel free to open a GitHub issue and I will do my best to help!   
