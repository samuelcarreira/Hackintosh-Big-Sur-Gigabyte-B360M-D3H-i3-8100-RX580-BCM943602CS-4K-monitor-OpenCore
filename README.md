# Hackintosh-Catalina-Gigabyte-B360M-D3H-i3-8100-RX580-BCM943602CS-4K-monitor-OpenCore

## *NOTE: This is a work in progress*

## Versions
macOS Catalina 10.15.5
OpenCore 0.5.9

## What's working
|       | Status | Aditional details |
| ----------- |  :----: | ----------- |
| Sound  | OK  |   |
| USB Ports  | OK  | I am using X USB 2.0 and 3.0...  |
| WiFi  | OK  |   |
| Bluetooth  | OK  |   |
| Airdrop/Handoff  | OK  |   |
| Ethrnet | OK |
| Unlock with Apple Watch | OK  |   |
| Airdrop/Handoff  | OK  |   |
| Graphics acceleration (dGPU) | OK?  | Connected to two monitors through DisplayPort and HDMI. I didn't compare the performance  |
| Sidecar  | No  |  iPad shows a black screen |
| Restart/Shutdown  | OK  |   |
| Sleep  | OK  |   |
| CPU power managment  | ?  | Not tested  |
| iServices | OK  |   |

## Problems
- none

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

### Bios Settings
...


## Credits
https://github.com/acidanthera/OpenCorePkg
https://www.reddit.com/r/hackintosh/
...
