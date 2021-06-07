# Hackintosh-Intel-i9-10900k-Gigabyte-Z490-AirDrop-AMD-580-IGPU

Hello there,

I have successfully installed MacOS Catalina 10.15.4 on my i9-10850k running on a Gigabyte Z490 ATX and Mini-ITX.

You can find my EFI/Config folder in this repository.

Bootloader: OpenCore 0.6.3 /0.6.7


# My Hardware
Intel i9-10850k
Mainboard: GIGABYTE Z490M GAMING X 
RAM: 32GB Corsair 3200 CL16
GPU: AMD Sapphire RX 580
Wifi/BT: MQUPIN fenvi T919 Wireless Card with BCM94360CD 


# What is Working
 Tested with macOS Catalina 10.15.6 and macOS Big Sur
 Graphics: IGPU and AMD RX 580 Working fine.
 Wifi and Bluetooth via BCM94360CD.
 Audio: Working by hisself. 
 USB-C Working
 Ethernet
 iCloud
 Programs: VM-Fusion, Microsoft Teams, Citrix, WhatsAPP, Telegram, 
 Games like : LoL, CS:GO, Diablo 3, WoW, MineCraft.
 Sleep/Wake
 Shutdown
 Restart

 
 
 
# Installation 
Create an MacOS Catalina 10.15.6 USB-Installer Stick. Do this on a real Mac.

Follow this Guide and Download Method: -> https://github.com/corpnewt/gibMacOS <-


<li> Plugin USB-Stick with at least 16GB. My installation needed 8.30 GB. </li>
<li> The following assumes your USB stick is called "USB_NAME" Normality is "MyVolume". </li>
<li> Check that "USB_NAME"/"MyVolume" is partitioned with GUID. </li>
<li> Open the terminal and enter this command to create the installer (Replace "USB_NAME"/"MyVolume" with your USB name. In this case Untitled. </li>
<li> sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/USB_NAME or MyVolume </li>
<li> At the end your USB should be named "Install macOS Catalina". </li>

# config.plist
if you use mine plist, dont forget to change the serial number. 
change the NEW_HERE with your serial number.

use this tool to genereate one. -> https://github.com/corpnewt/GenSMBIOS <-

if you have question join our Discord :)

# Discord
Join our discord to be one of the first to receive updates and news to anything tech!

https://discord.gg/DDXmRxXX8Y


# Thanks to:
https://github.com/corpnewt
