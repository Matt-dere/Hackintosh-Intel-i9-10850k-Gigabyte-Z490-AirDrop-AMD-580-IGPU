# Hackintosh-Intel-i9-10900k-Gigabyte-Z490-AirDrop-AMD-580-IGPU

Hello there,

I have successfully installed MacOS Catalina 10.15.4 on my i9-10850k running on a Gigabyte Z490 ATX and Mini-ITX.

You can find my EFI/Config folder in this repository.

Bootloader: OpenCore 0.6.3 /0.6.7


# My Hardware
<li> Intel i9-10850k </li>
<li> Mainboard: GIGABYTE Z490M GAMING X </li>
<li> RAM: 32GB Corsair 3200 CL16 </li>
<li> GPU: AMD Sapphire RX 580 </li>
<li> Wifi/BT/AirDrop: MQUPIN fenvi T919 Wireless Card with BCM94360CD </li>


# What works so far
<li> Tested with macOS Catalina 10.15.6 and macOS Big Sur </li>
<li> Graphics: IGPU and AMD RX 580 Working fine. </li>
<li> Wifi,Bluetooth and AirDrop via BCM94360CD. </li>
<li> Audio: Working by hisself. </li>
<li> USB-C Working </li>
<li> Ethernet </li>
<li> iCloud </li>
<li> Application: VM-Fusion, Microsoft Teams, Citrix, WhatsAPP, Telegram, </li>
<li> Games like : LoL, CS:GO, Diablo 3, WoW, MineCraft. </li>
<li> Sleep/Wake </li>
<li> Shutdown </li>
<li> Restart </li>

 
 
 
# Installation 
Create an MacOS Catalina 10.15.6 USB-Installer FlashDrive. Do this on a real Mac.

Follow this Guide and Download Method: -> https://github.com/corpnewt/gibMacOS <-


<li> Plugin USB-Drive with at least 16GB. My installation needed 8.30 GB. </li>
<li> The following assumes your USB stick is called "USB_NAME" Normality is "MyVolume". </li>
<li> Check that "USB_NAME"/"MyVolume" is partitioned with GUID. </li>
<li> Open the terminal and enter this command to create the installer (Replace "USB_NAME"/"MyVolume" with your USB name. In this case Untitled. </li>
<li> sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume </li>
<li> At the end your USB should be named "Install macOS Catalina". </li>

# config.plist
if you use my plist, don’t forget to change the serial number. Change the NEW_HERE accordingly with your serial number.

use this tool to genereate one. -> https://github.com/corpnewt/GenSMBIOS <-


# Bios Settings
Skip steps with setting you can’t find in your BIOS
<li> ----> Disable <---- </li>

<li> Fast Boot </li>
<li> Secure Boot </li>
<li> Serial/COM Port </li>
<li> Parallel Port </li>
<li> VT-d (can be enabled if you set DisableIoMapper to YES) </li>
<li> CSM </li>
<li> Thunderbolt(For initial install, as Thunderbolt can cause issues if not setup correctly) </li>
<li> Intel SGX </li>
<li> Intel Platform Trust </li>
<li> CFG Lock (MSR 0xE2 write protection)(This must be off, if you can't find the option then enable AppleXcpmCfgLock under Kernel -> Quirks. Your hack will not boot with CFG-Lock enabled) </li>



<li> ----> Enable <---- </li>

<li> VT-x </li>
<li> Above 4G decoding </li>
<li> 2020+ BIOS Notes: When enabling Above4G, Resizable BAR Support may become an available on some Z490 and newer motherboards. Please ensure this is Disabled instead of set to Auto. </li>
<li> Hyper-Threading </li>
<li> Execute Disable Bit </li>
<li> EHCI/XHCI Hand-off </li>
<li> OS type: Windows 8.1/10 UEFI Mode </li>
<li> DVMT Pre-Allocated(iGPU Memory): 64MB </li>
<li> SATA Mode: AHCI </li>




# Discord
Join our discord to be one of the first to receive updates and news to anything tech!

https://discord.gg/kQtzkqhD


# Thanks to:
https://github.com/corpnewt
