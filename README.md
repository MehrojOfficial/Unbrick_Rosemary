# Unbrick RN10S/11SE Indian/Poco M5S

All about unbricking REDMI NOTE 10S/11SE(India)/Poco M5s

## USE THIS GUIDE AT YOUR OWN RISK. I AM NOT RESPONSIBLE TO YOUR ALREADY HARD OR SOFT BRICKED DEVICE

All the required files:
- [Download](https://www.pling.com/p/1953522)

**What are the requirements:**
1. Windows 10 operating sytem (Windows 11 didn't work, better not to try it);
2. Active network connection;
2. Discipline to follow the steps & Big brain & Patience.

**When to use this unbricking method:**
1. If your device bootlooping and can't access fastboot and recovery. Try to boot fastboot/recovery with differently timed key combinations. 
		(If you can format data or reflash stock fastboot rom, do it or else you just waste your time with it);
2. The device is not even turning on.
		(In this case this method probably fail but it depends, so give it a shot as a last hope before going to service).

**What should be considered before this method:**
1. If your device in this condition, you already lost your data. Don't even think about recovering it.
2. It works on both bootloader conditions: locked and unlocked.
3. Despite your bootloader was locked or unlocked before the process, your bootloader will be locked after this process.

#### Step 1: 
- First of all let bootloop to drain your battery completely.(You can actually skip it try if you have more power left);

#### Step 2:
- Unzip the downloaded 'HardBrickFixRN10S.zip' file and place it somewhere easy to use.

#### Step 3:
- Download and extract stock fastboot firmware not customs please;

#### Step 4:	
- Go to 'HardBrickFixRN10S/Python';
- Install Python V3.9.7 (MUST TICK 'Add Python 3.9 to PATH' option while installing);
- Double-click on 'add_requirements.bat' to download libraries.

#### Step 4:
- Go to 'HardBrickFixRN10S/Drivers';
- Install 'MTK_Driver_Installer.exe' by following installion-wizard;
- AFTER THIS STEP PC MUST BE RESTARTED;

#### Step 5:	
- Go to 'HardBrickFixRN10S/Drivers';
- Right-click on 'cdc-acm.inf'and click 'Install' on opened menu;

#### Step 6:	
- Go to 'HardBrickFixRN10S/LibUSB';
- Install 'LibUSB-1.2.6.0.exe' by by following installion-wizard;
- After it launched select "Install a device filter";
		
#### Step 7: Here you need to be really quick:
- After this, connect your phone to the pc with usb while holding volume down button;
- Click 'Next';
#### As soon as you see the device with the name of "MediaTek USB Port", select and install it immediately;
- If it fails or device boots up before you do anything, repeat this step multiple times till it works;
- If you see success message from the app, remove your phone from PC.

___

**In the Step-8,**
- **If it succeeds, your phone will stop bootlooping which is good but,**
**<br>DO NOT TOUCH YOUR PHONE, DO NOT DISCONNECT IT FROM THE COMPUTER,**
**<br>just put your phone next to you, and continue with the guide.**

- **If it fails, try to do it untill it works.**
___
#### Step 8:
- Go to 'HardBrickFixRN10S/Bypass';
- Double click on 'BYPASS.bat';
- If you see "Waiting for device", connect your phone to PC holding volume down button;
- If the process outputs with "Found port = COM3" and 'Protection disabled', it means it was successful;
- Don't unplug the device from pc, look at the warning above Step-8 again, it is very important.

#### Step 9:
- Go to 'HardBrickFixRN10S/SPFlashTool';
- Open 'flash_tool.exe' (Click OK if it shows error)

#### Step 10:
In SpFlashTool:
- for 'Download-Agent' select 'No-Auth.bin' in the same directory;
- for 'Scatter-loading File' go to {FastbootRom}/images and select {MT6785_Android_scatter.txt};
- Change drop-down from 'Download Only' to 'Firmware Upgrade';
- Click 'Download' and wait till it displays big green stick icon.

> {FastbootRom} - the upper location of your extracted firmware.
<br>{MT6785_Android_scatter.txt} - the scatter filename might be different, however it always ends with 'xxxxxx_Android_scatter.txt'.

#### Step 11:
- After SpFlashTool finishes remove your phone from PC;
- Finally turn it on;
___
THAT'S ALL TO RECOVER UNBRICKED REDMI NOTE 10S/11SE(INDIA)/POCO M5S FROM SCRATCH.
<br>NOW COMPLETE SETUP AND CONSIDER THAT YOUR BOOTLOADER IS LOCKED.
<br>NEVER DO THAT MISTAKES AGAIN, NOW ENJOY.
		
