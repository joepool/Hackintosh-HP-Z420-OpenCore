# Hackintosh-HP-Z420-OpenCore
Hackintosh EFI for HP Z420 Workstation Using Catalina/Big Sur Beta   
I am currently doing a conversion from Clover to OpenCore  and i have Catalina working with Clover  
This is currently not working, at the moment this repo is for me to keep track of things...   
I will update when I can boot.  

# My System
Intel Xeon E5-1650 v2 CPU  
Nvidia Quadro K4000 GPU   
32GB ECC DDR3   

# Issues    
`apfs_module_start:1689: load: com.apple.filefsytem.apfs, v1412.120.2, apfs-1412.120.2`    
`[EB|#LOG:EXITBS:START]`    
`still waiting for root device`
    
See Error Images/Boot Log for full errors.    


# Troubleshooting Steps Taken.  

Everything here: https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/troubleshooting.html#stuck-on-eb-log-exitbs-start     
Everything here: https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/troubleshooting.html#stuck-on-rtc-pci-configuration-begins-previous-shutdown-hpet-hid-legacy     
I have SSDT-EC.aml - I have tried the premade one and one i made with SSDTTime. Tried changing loads of qwerks etc, nothing worked...    
    

Reddit Discussion on Issues i am having: https://www.reddit.com/r/hackintosh/comments/i52se0/clover_to_opencore_conversion_help_catalina/
