# Hackintosh EFI for HP ProBook 650 G5

> 🇷🇺 [Читать на русском языке](./README.ru.md)

Fully working EFI for macOS Ventura / Sonoma (tested), configured for HP ProBook 650 G5.

> ⚠️ Stability: ~95%  
> - Not working: card reader, fingerprint scanner, AirDrop / AirPlay / Handoff

---

## 📋 System Specifications

| Component           | Description                                  |
|---------------------|----------------------------------------------|
| Laptop Model        | HP ProBook 650 G5 (7YL73ES)                  |
| CPU                 | Intel Core i5-8365U (Whiskey Lake)           |
| Graphics            | Intel UHD Graphics 620                        |
| RAM                 | 16 GB DDR4                                   |
| Audio               | Realtek ALC236 (layout-id 13)                 |
| Wi-Fi               | Intel Dual Band Wireless-AC 9560              |
| Ethernet            | Intel I219-V (works via IntelMausi)          |
| Touchpad            | Synaptics (via VoodooPS2Controller)           |
| Screen              | 15.6" FHD                                    |
| Video Output        | HDMI Audio/Video ✅                           |
| USB                 | All ports working without custom USB map ✅  |
| Camera              | Built-in, working ✅                          |
| Bluetooth           | Intel module, limited support                 |
| Card Reader         | BayHubTech SD Reader ❌                       |
| Fingerprint Scanner | ❌                                            |
| Wi-Fi GUI / Airport | AirportItlwm.kext ✅ (no AirDrop)             |

---

## ✅ Working

- iMessage and FaceTime  
- Intel UHD 620 graphics (including HDMI audio)  
- Sleep / Wake  
- USB ports (work without custom USB mapping)  
- Keyboard / Touchpad (Synaptics via VoodooPS2Controller)  
- Audio via AppleALC  
- Wi-Fi via AirportItlwm.kext  
- Camera  
- Ethernet (IntelMausi)  

---

## ❌ Not Working

- Card reader (BayHubTech)  
- Fingerprint scanner  
- AirDrop / Handoff / AirPlay (Intel Wi-Fi)  

---

## 🔧 Installation Notes

- Using OpenCore (version 1.0.4)  
- Installed via official macOS installer  
- Custom SSDTs used: `SSDT-USBX`, `SSDT-PNLF`, `SSDT-AWAC`, `SSDT-PLUG`  

---

## 🔄 Future Improvements

- Testing card reader support (via `Sinetek-rtsx` or `HackrNVMe`) — no success yet  
- Possible Wi-Fi module replacement to Broadcom BCM94360NG for full compatibility  

---

> This build is still in progress. Pull requests are welcome!
