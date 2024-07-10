# Run MacOS 13 Ventura on Lenovo ThinkPad P52 (20M90017FR) 
This is my backup EFI for running MacOS Ventura on my Thinkpad P52. 

On Windows/Linux all you need is downloading Ventura using `macrecovery.py`, make a bootable USB and place this EFI on the root of the USB drive. For more information follow Dortania guide : https://dortania.github.io/OpenCore-Install-Guide

### Specifications
- CPU: 8th Generation Intel Core i7-8850H (Coffee-Lake) 
- GPU: Intel UHD Graphics 630 + Nvidia P1000 (disabled) 
- CHIPSET: Mobile Intel CM246 Chipset
- WLAN/BT: Intel Wireless-AC 9560
- AUDIO CODEC:  ALC3286 codec

### What's not working
... basically everything is stable except :
- ❌ External HDMI display: the HDMI output is probably physically linked to the Nvidia P1000 (which is not compatible with MacOS).
- ❌ USB-C/Thunderbolt: with Thunderbolt enabled, the system restarts few seconds after disconnecting a USB-C cable, so i had to disable Thunderbolt in BIOS.
- ❌ SD Card Reader (haven't investigated any further)
- ❌ Trackpoint (i never used it)
- ❌ Fingerprint reader (i also don't care)

Note: All Kexts are in DEBUG mode, if everything's ok make sure to replace them with their RELEASE packages
