# Hackintosh-HP-Z420-OpenCore
Hackintosh EFI for HP Z420 Workstation Using Catalina/Big Sur Beta   
I am currently doing a conversion from Clover to OpenCore  and i have Catalina working with Clover  
This is currently not working, at the moment this repo is for me to keep track of things...   
I will update when I can boot.  

# Current Progress:    
It Boots MacOS Catalina! I havent tested everything yet, but once i have and fixed any issues, i will update this page.    
It Boots MacOS BigSur DB4! Again, not sure if everything works yet, but i will update when I know it does.   

# My System
Intel Xeon E5-1650 v2 CPU  
Nvidia Quadro K4000 GPU   
32GB ECC DDR3   

# Issues   
~~Power Management.~~ Fixed   
~~Audio.~~ Fixed    
USB3. - The Z420 uses a Texas Instruments USB 3 Controller which is unsupported in MacOS   
DRM. - My GPU is incompatable so DRM will never work for me.   
Internal Speaker.    
~~Current issue i am facing - discussion on reddit: https://www.reddit.com/r/hackintosh/comments/i66pqf/clover_to_opencore_conversion_help_keep_getting/~~ **Fixed!!**     
     
~~`apfs_module_start:1689: load: com.apple.filefsytem.apfs, v1412.120.2, apfs-1412.120.2`~~    
~~`still waiting for root device`~~   
~~I believe what is causing these issues is something to do with usb ports, i get past this message when i boot the macos installer from an internal sata hard drive. Diangnostics for this in progress now~~ **Fixed!!**     
