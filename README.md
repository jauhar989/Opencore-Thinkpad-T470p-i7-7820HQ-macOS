# Opencore-Thinkpad-T470p-i7-7820HQ-macOS
macOS Opencore Bootloader Configuration for Thinkpad T470p i7-7820HQ series with NVIDIA 940MX

## Specification
Specification | Configuration
----------- | -----------
Processor | Intel Core i7-7820HQ
Integrated Graphics | Intel HD Graphics 630
Dedicated Graphics | NVIDIA GeForce 940MX 2GB
Memory | SAMSUNG Dual-Channel 32GB
Storage | 256GB Lightning SSD M.2 SATA
Wireless Card | Intel AC-8260 Dual Band + Bluetooth
Bootloader | OpenCore
Bootloader Ver. | v0.9.6

## Screenshot
<p align="center">
  <kbd><img src="https://raw.githubusercontent.com/jauhar989/Opencore-Thinkpad-T470p-i7-7820HQ-macOS/main/Screenshot/T470p-ventura-about-mac.png"/></kbd></kbd>
<p align="center">
  <kbd><img src="https://raw.githubusercontent.com/jauhar989/Opencore-Thinkpad-T470p-i7-7820HQ-macOS/main/Screenshot/T470p-ventura-sys-monitor.png"/></kbd></kbd>
</p>
<p align="center">
  <kbd><img src="https://github.com/jauhar989/Opencore-Thinkpad-T470p-i7-7820HQ-macOS/blob/main/Screenshot/T470p-ventura-system-info-hackintool.png"/></kbd></kbd>
</p>

### Before you start
Follow dortania guide on how to create a recovery usb for MacOS installation.
You can find the MacOS installation guide at the following link, [`click here`](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html#downloading-macos)

## MacOS
- Ventura (Tested, OpenCore)

# Bios
- `Security -> Security Chip`: **Disabled**;
- `Memory Protection -> Execution Prevention`: **Enabled**;
- `Virtualization -> Intel Virtualization Technology`: **Enabled**;
- `Virtualization -> Intel VT-d Feature`: **Disabled**;
- `Internal Device Access -> Bottom Cover Tamper Detection`: must be **Disabled**;
- `Anti-Theft -> Computrace -> Current Setting`: **Disabled**;
- `Secure Boot -> Secure Boot`: **Disabled**;
- `UEFI/Legacy Boot`: **UEFI Only**;
- `CSM Support`: **No**.

## What's Working?
- Intel HD Graphics 630 `Ventura`
- Power Management `Ventura`
- Shutdown, Restart `Ventura`
- Audio Speaker & Earphone `Ventura`
- Bluetooth `Ventura`
- Trackpad, Trackball, Gestures `Ventura`
- Battery Indicator `Ventura`
- Camera `Ventura`

## Not Tested
- Docking Station
- HDMI

## Bug
- The Brightness control is working but the keyboard buttons are not working yet. *Will be fixed soon*
- Sleep works, but sometimes black screen when waking up. However, this can be resolved if the laptop screen is closed and then reopened. *Will be fixed soon*
- Samsung PM981a NVME SSD causes kernel panic during installation.
- Touchscreen is not working yet.

## Credits:
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/)
- [EliteMacx86](https://www.youtube.com/@EliteMacx86)
