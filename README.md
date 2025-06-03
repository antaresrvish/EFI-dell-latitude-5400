# Dell Latitude 5400 Hackintosh OpenCore EFI

This repository contains OpenCore EFI files for running macOS Ventura on Dell Latitude 5400. This EFI is provided as-is. Use at your own risk.

## 💻 Hardware Specifications

| Component | Details |
|-----------|---------|
| Model | Dell Latitude 5400 |
| CPU | Intel Core i5-8365U Whiskey Lake |
| GPU | Intel UHD Graphics 630 |
| RAM | 24GB DDR4 2400MHz |
| Storage | WDC SN520 NVMe 256GB SSD |
| Display | 14" 1920x1080 |
| Audio | Realtek ALC236 |
| Network | Intel Wireless-AC 9560 |

## ✅ Working Features

- [x] CPU Power Management
- [x] Wi-Fi & Bluetooth
- [x] USB Ports
- [x] Trackpad with Gestures
- [x] Built-in Keyboard
- [x] HDMI
- [x] Audio (Input/Output)
- [x] Built-in Camera
- [x] Ethernet
- [x] Sleep/Wake
- [x] Backlight Control

## ⚠️ Known Issues

- bluetoothd daemon crash after sleep, (fixable by killing bluetoothd process)

## ❔ Not Tested

- SIM Card Reader
- SD Card Reader

## 📝 Post-Installation 

1. Generate SSDT tables using SSDTTime
   - Follow [Dortania's ACPI Guide](https://dortania.github.io/Getting-Started-With-ACPI/ssdt-methods/ssdt-easy.html)

## 🗂️ EFI Folder Structure

- BOOT/
  - BOOTx64.efi
- OC/
  - OpenCore.efi
  - config.plist
  - ACPI/ (SSDT files)
  - Drivers/ (Required EFI drivers)
  - Kexts/ (Required kernel extensions)
  - Resources/ (OpenCore interface resources)