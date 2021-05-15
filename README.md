# Hackintosh-dell-inspiron-5559

**OC Version - 0.6.9**

**MacOS Version - 11.3.1**


![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/Screenshots/Screenshot%202021-05-11%20at%202.38.58%20PM.png?raw=true)


## System Configuration :-
Specifications | Details
-------------- | -------------
Laptop Model | Dell Inspiron 5559
Processor | I3 - 6100U @ 2.3GHZ Dual Core
Graphics | Intel HD Graphics 520
Ram | 2 x 4 GB
Audio Codec | ALC255
Keyboard | PS/2
Trackpad | I2CHID / PS/2 Compatible
Ethernet | RealTek RTL810xE
WIFI Card | Intel Dual Band Wirelss AC-3160

## What's Working :
- Intel HD Graphics 520 
- Audio : 
-   - Internal Speaker out, Headphone out
-   - Internal Mic In, Headphone Mic in 
- Battery Indicator
- Sleep + Wake + Restart + Shutdown
- Brightness Slider and Brightness Fn key [ F11, F12]
- Imessage + Facetime + Icloud + App Store
- Trackpad with both **I2CHID** And PS/2
- All USB Ports - 1 x USB 3.0, 2 x USB 2.0
- HDMI + HDMI Audio
- Ethernet
- WIFI + Bluetooth
- Boot Chime

## What's Not Working :

- Sd Slot
- ....


## Create Bootable Pen Drive :
- Follow [this](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/) guide 

## How to edit the config.plist
- [Download] (https://github.com/corpnewt/ProperTree)
- Make Any Changes using propertree or you can even use any TextEditor


## Generate your serial
- Download [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) / Use [Macserial](https://github.com/acidanthera/OpenCorePkg/releases) 
- Generate a SMBIOS for Macbookpro13,1 and add the serials to the config.plist
- Use only Invalid serial check at this [site](https://checkcoverage.apple.com/in/en/)


![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/Screenshots/Screenshot%202021-05-11%20at%2011.20.03%20AM.png?raw=true)



## Change these settings in BIOS : -
- - Enable
- - VT-x
- - Above 4G decoding
- - Hyper-Threading
- - Execute Disable Bit
- - EHCI/XHCI Hand-off
- - OS type: Windows 8.1/10 UEFI Mode
- - DVMT Pre-Allocated(iGPU Memory): 64MB
- - SATA Mode: AHCI

## For More Info :
- For more Info [**Visit**](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#starting-point) this site
- or feel free to create a new issue

## Get your Headset Mic working

1. Download [ComboJackInstaller ](https://github.com/hackintosh-stuff/ComboJack)
2. Use the Install Script under ComboJack_Installer
3. Do not change the Layout if you need to change the layout try 71 or 86
4. Reboot

## Control FAN Speed

- Download [Macs Fan Control](https://crystalidea.com/macs-fan-control?ref=macupdate)

    Use Mac's Fan Control.app
    Use Pro Version with :
      Gmail : macwk.com@gmail.com
      License Key : MPD8G-XGA1C-WMDYE-WYCYY-FPX6W-TS1J8-P9P71-7GTPB-V6RAH-2B42R-PD1C8

## Post install fixes : 
- [Fixing Iservices](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)
- [Booting with out USB](https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html)
- [Fixing Power Management](https://dortania.github.io/OpenCore-Post-Install/universal/pm.html)
- [Fixing Sleep](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html)
- [Fixing USB Power](https://dortania.github.io/OpenCore-Post-Install/usb/)
