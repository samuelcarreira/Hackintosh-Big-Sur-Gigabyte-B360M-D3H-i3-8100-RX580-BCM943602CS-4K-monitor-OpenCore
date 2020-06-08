# Hackintosh-Catalina-Gigabyte-B360M-D3H-i3-8100-RX580-BCM943602CS-4K-monitor-OpenCore

## *NOTE: This is a work in progress*

## Versions
macOS Catalina 10.15.5
OpenCore 0.5.9

## What's working
||Status|Additional details|
|:-|:-|:-|
|Sound|OK||
|USB Ports|OK|6 x USB 2.0; 4 x USB 3.0: I didn't perform any speed test on the USB 3.1 port|
|WiFi|OK||
|Bluetooth|OK||
|Airdrop/Handoff|OK||
|Ethernet|OK||
|Unlock with Apple Watch|OK||
|Airdrop/Handoff|OK||
|Graphics acceleration (dGPU)|OK?|Connected to two monitors through DisplayPort and HDMI. I didn't compare the performance|
|Sidecar|No|iPad shows a black screen|
|Restart/Shutdown|OK||
|Sleep|OK||
|CPU power management|?|Not tested|
|iServices|OK||
|DRM| OK?| Apple TV works well but the mouse cursor disappears. Netflix starts to play but after some seconds the video turns black|


## Complete hardware description
- Gigabyte B360M D3H
- Intel i3-8100 @3.60GHz
- Sapphire Radeon RX 580 Nitro+
- 2x4GB DDR4 2400MHz
- Wifi and Bluetooth card (PCI-express 1x adapter BCM943602CS
- Dual monitor setup:
  - 4K monitor (DisplayPort)
  - 1080p vertical monitor (HDMI)
- Dual boot system
  - 500GB SSD for Windows/Linux
  - 128GB SDD only for MacOS


## Dual boot
Because I mainly use Windows and Linux (for professional reasons) I didn't need a quick dual boot setup. So I use a cheap SSD for macOS. When I want to boot on macOS, I press F12 to select the BIOS startup disk.

## Material required
- *16GB USB Flash Drive* The new macOS Catalina doesn't fit anymore on a 8GB flash drive, because I had problems on the past with my USB 3.0 flash drive, I use an old USB 2.0 flash drive to hackintosh

## Instructions
Follow the guide https://dortania.github.io/OpenCore-Desktop-Guide/

## EFI Folder
```
├───BOOT
│       BOOTx64.efi
│       
└───OC
    │   config.plist
    │   OpenCore.efi
    │   
    ├───ACPI
    │       SSDT-AWAC.aml
    │       SSDT-EC.aml
    │       SSDT-PLUG.aml
    │       SSDT-PMC.aml
    │       SSDT-SBUS-MCHC.aml
    │       SSDT-USBX.aml
    │       
    ├───Bootstrap
    │       Bootstrap.efi
    │       
    ├───Drivers
    │       AudioDxe.efi
    │       CrScreenshotDxe.efi
    │       HfsPlus.efi
    │       OpenRuntime.efi
    │       
    ├───Kexts
    │   ├───AppleALC.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       └───MacOS
    │   │               AppleALC
    │   │               
    │   ├───IntelMausi.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       └───MacOS
    │   │               IntelMausi
    │   │               
    │   ├───Lilu.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       └───MacOS
    │   │               Lilu
    │   │               
    │   ├───SMCProcessor.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       └───MacOS
    │   │               SMCProcessor
    │   │               
    │   ├───SMCSuperIO.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       └───MacOS
    │   │               SMCSuperIO
    │   │               
    │   ├───USBInjectAll.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       ├───MacOS
    │   │       │       USBInjectAll
    │   │       │       
    │   │       └───_CodeSignature
    │   │               CodeResources
    │   │               
    │   ├───VirtualSMC.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       └───MacOS
    │   │               VirtualSMC
    │   │               
    │   ├───WhateverGreen.kext
    │   │   └───Contents
    │   │       │   Info.plist
    │   │       │   
    │   │       └───MacOS
    │   │               WhateverGreen
    │   │               
    │   └───XHCI-unsupported.kext
    │       └───Contents
    │               Info.plist
    │               
    ├───Resources
    │   ├───Audio
    │   ├───Font
    │   ├───Image
    │   └───Label
    └───Tools
            OpenShell.efi
```

### Bios Settings
TODO


## Credits
- https://github.com/acidanthera/OpenCorePkg
- https://www.reddit.com/r/hackintosh/

