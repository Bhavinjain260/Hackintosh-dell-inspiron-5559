# Hackintosh-dell-inspiron-5559



**Do Not Clone And Use The EFI.** 

**Download From Release Tab**

**This EFI is unTested**

**OC Version - 0.7.9**

**Latest Stable MacOS Version supported - 12.3**


![About this Mac](https://user-images.githubusercontent.com/49932650/155383613-cd7aed4e-c0b5-4f99-8cf1-c405b863c980.png)


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
- SD Card Reader

## What's Not Working :

- ....


## Changes You Need To Make :- 

<details>
<summary><strong>How to edit the config.plist
</strong></summary>
    
1. [Download] (https://github.com/corpnewt/ProperTree)
2. Make Any Changes using propertree or you can even use any TextEditor
</details>


<details>
<summary><strong>Change these settings in BIOS</strong></summary>
    
- Enable
- VT-x
- Above 4G decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: Windows 8.1/10 UEFI Mode
- DVMT Pre-Allocated(iGPU Memory): 64MB
- SATA Mode: AHCI
    
</details>




<details>
<summary><strong>Generate a Serial</strong></summary>
    
1. Download and open [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
    
    
![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/SMBios/1.png?raw=true)
    
    
2. Select 3 to Genrate SMBios with ROM
    
    
![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/SMBios/2.png?raw=true)
    
    
3. Now Type "MacBookPro13,1 5" / "MacBookPro13,2 5" this will genarate 5 SMBios with ROM
    
    
![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/SMBios/3.png?raw=true)
    
![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/SMBios/4.png?raw=true)
    
    
4. Check the Serial validity on [Apple's check coverage](https://checkcoverage.apple.com/in/en/) **We have to use only invalid serial**

![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/SMBios/5.png?raw=true)
    
    
5. Copy the serial in the config
    - **Type** Goes in **Generic -> SystemProductName**
    - **Serial** goes in **Generic -> SystemSerialNumber**
    - **Board Serial** goes in **Generic -> MLB**
    - **SmUUID** part goes in **Generic -> SystemUUID**
    - **Apple Rom** goes in **Generic -> ROM**
    
    
![Alt text](https://github.com/Bhavinjain260/Hackintosh-dell-5559-opencore/blob/main/SMBios/6.png?raw=true)
    
</details>




<details>
<summary><strong>Get your Headset Mic working
</strong></summary>
    
1. Download [ComboJackInstaller ](https://github.com/hackintosh-stuff/ComboJack) [ComboJackInstaller Test version](https://github.com/Bhavinjain260/ComboJack)
2. Use the Install Script under ComboJack_Installer
3. Reboot
</details>


<details>
<summary><strong>Control Fan Speed</strong></summary>
    
- Download [MAC'SFANCONTROL](https://crystalidea.com/macs-fan-control?ref=macupdate)

    Use Mac's Fan Control.app
    Use Pro Version with :
      Gmail : macwk.com@gmail.com
      License Key : MPD8G-XGA1C-WMDYE-WYCYY-FPX6W-TS1J8-P9P71-7GTPB-V6RAH-2B42R-PD1C8
</details>

