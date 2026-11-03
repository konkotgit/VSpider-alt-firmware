# 🕷️ VSpider – Alternative Firmware & ROM

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
2. To enter the setup menu, hold **CAPS SHIFT** during the startup screen.
3. Use **Q / A** to navigate through the menu options.
4. Press **SPACE / ENTER** to change the selected option.
5. Select **BOOT WITH THESE SETTINGS** and press **SPACE / ENTER** to apply the configuration and start the machine.

**Additional information:**
- If CAPS SHIFT is not pressed, the machine boots automatically using the current CPLD configuration.
- The setup menu always starts with default configuration values.
- Selecting ZX Spectrum +3 automatically selects +3e MMC (Z-Controller).
- Selecting ZX Spectrum 128K or ZX Spectrum 48K automatically selects DivMMC.
- Configuration changes are not saved and remain active only until power-off.

---

## 📝 Changelog

- **Rev. 1.1**
  Initial public release.

---

## 🔧 Hardware Configuration

The right-hand DIP switch forces ZX Spectrum 48K mode and disables the setup menu. This ensures compatibility with external interfaces, particularly disk interfaces.

---

## ⚠️ Known Issues

- Floating bus logic is not implemented in the CPLD yet.

---

## 🎥 Demo Video

Coming soon! ;)