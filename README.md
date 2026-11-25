

# OpenCore EFI for Lenovo ThinkPad X230 - macOS Ventura 13.7.4

EFI folder tested for running **macOS Ventura 13.7.4** on a **Lenovo ThinkPad X230** with **OpenCore 1.0.9**.

## Hardware & Features Summary

- **Specs:** Intel Core i5-3320M, Intel HD Graphics 4000, 8 GB RAM, Intel Wi-Fi / Ethernet, SMBIOS MacBookPro14,1.
- **Working:** Graphics acceleration, audio, keyboard/trackpoint/touchpad, USB ports, and network/Wi-Fi (`AirportItlwm`).
- **Known Issues:** Bluetooth is untested/failing on the test unit; Sleep/Wake is not fully verified (using *Caffeine* to prevent sleep).

## Essential Pre-Use Steps

1. **Generate unique SMBIOS data:** Update `PlatformInfo -> Generic` in `config.plist` (`SystemSerialNumber`, `MLB`, `SystemUUID`, `ROM`) keeping the **MacBookPro14,1** profile.
2. **Backup:** Keep a backup of your current working EFI on a USB stick.
