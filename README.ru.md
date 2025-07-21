# Hackintosh EFI для HP ProBook 650 G5

> 🇬🇧 [Read in English](./README.md)

Полностью рабочее EFI для macOS Ventura / Sonoma (проверено), настроенное для HP ProBook 650 G5.

> ⚠️ Работоспособность: ~95%  
> — Не работает: кардридер, сканер отпечатков пальцев, AirDrop / AirPlay / Handoff

---

## 📋 Системные характеристики

| Компонент            | Описание                                   |
|----------------------|---------------------------------------------|
| Модель ноутбука      | HP ProBook 650 G5 (7YL73ES)                |
| Процессор            | Intel Core i5-8365U (Whiskey Lake)         |
| Графика              | Intel UHD Graphics 620                     |
| ОЗУ                  | 16 GB DDR4                                 |
| Аудио                | Realtek ALC236 (layout-id 13)              |
| Wi-Fi                | Intel Dual Band Wireless-AC 9560           |
| Ethernet             | Intel I219-V (работает через IntelMausi)   |
| Тачпад               | Synaptics (через VoodooPS2Controller)      |
| Экран                | 15.6" FHD                                   |
| Видеовыход           | HDMI Audio/Video ✅                         |
| USB                  | Все порты работают без карты ✅             |
| Камера               | Встроенная, работает ✅                     |
| Bluetooth            | Через Intel модуль, ограниченно            |
| Кардридер            | BayHubTech SD Reader ❌                    |
| Сканер отпечатков    | ❌                                           |
| Wi-Fi GUI / Airport  | AirportItlwm.kext ✅ (без AirDrop)         |

---

## ✅ Работает

- iMessage и FaceTime  
- Графика UHD 620 (включая HDMI аудио)  
- Sleep / Wake  
- USB порты (работают без необходимости кастомной карты)  
- Клавиатура / Тачпад (Synaptics через VoodooPS2Controller)  
- Аудио через AppleALC  
- Wi-Fi через AirportItlwm.kext  
- Камера  
- Ethernet (IntelMausi)

---

## ❌ Не работает

- Кардридер (BayHubTech)  
- Сканер отпечатков пальцев  
- AirDrop / Handoff / AirPlay (Intel Wi-Fi)

---

## 🔧 Заметки по установке

- Используется OpenCore (версия 1.0.4)  
- Система установлена через оригинальный установщик macOS  
- Используются SSDT: `SSDT-USBX`, `SSDT-PNLF`, `SSDT-AWAC`, `SSDT-PLUG`

---

## 🔄 Будущие улучшения

- Проверка и возможный запуск кардридера (через `Sinetek-rtsx` или `HackrNVMe`) — пока безуспешно  
- Возможная замена Wi-Fi модуля на Broadcom BCM94360NG для полной совместимости с AirDrop / Handoff / AirPlay
