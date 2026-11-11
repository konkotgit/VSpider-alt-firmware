# 🕷️ VSpider – Alternative Firmware and ROM

Alternative firmware and ROM for the VSpider hardware.

---

## ⚙️ Features

**Three operating modes:**
- ZX Spectrum 128K
- ZX Spectrum 48K / Timex 2048
- ZX Spectrum +3 with +3e support

**Configuration options:**
- Machine mode selection
- DivMMC On/Off (ZX128 / ZX48 modes)
- DivMMC / +3e MMC selection (ZX +3 mode)
- TurboSound On/Off
- Kempston On/Off

Configuration changes are applied directly to the CPLD and remain active until the device is powered off.

**Default power-on configuration:**
- Machine mode: ZX Spectrum 128K
- DivMMC: On
- TurboSound: On
- Kempston: On

---

## 🎮 How to Use

1. Power on the VSpider. The startup screen is displayed for approximately 1.5 seconds.
2. To enter the setup menu, hold **CAPS SHIFT** while the startup screen is displayed.
3. Use **Q / A** to navigate through the menu options.
4. Press **SPACE / ENTER** to change the selected option.
5. Select **BOOT WITH THESE SETTINGS** and press **SPACE / ENTER** to apply the configuration and boot the machine.

**Additional information:**
- If CAPS SHIFT is not pressed, the machine boots automatically using the current CPLD configuration.
- The setup menu always starts with the default configuration values.
- Selecting ZX Spectrum +3 automatically selects +3e MMC.
- Selecting ZX Spectrum 128K or ZX Spectrum 48K automatically selects DivMMC.
- Configuration changes are not saved and remain active only until the device is powered off.

---

## 📝 Changelog

- **Rev. 1.1**  
  Initial public release.

---

## 🔧 Hardware Configuration

The right-hand DIP switch forces ZX Spectrum 48K mode and disables the setup menu. This ensures compatibility with external interfaces, particularly disk interfaces.

---

## ⚠️ Known Issues

- Floating bus logic has not yet been implemented in the CPLD.
- If the SD card is not detected in +3e mode, press RESET.

---

## 🎥 Demo Video

[![YouTube](https://img.youtube.com/vi/bjnyU8IcQSs/0.jpg)](https://www.youtube.com/watch?v=bjnyU8IcQSs)
