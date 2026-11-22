# 🕷️ VSpider – Alternative Firmware and ROM

Alternative firmware and ROM for VSpider hardware.

---

## ⚙️ Features

**Supported machine modes:**
- ZX Spectrum 128K
- ZX Spectrum +3 with +3e support
- ZX Spectrum 48K
- Timex TC 2048
- Pentagon 128 (DivMMC or Z-Controller when DivMMC is disabled)
- Pentagon 512 with Gluk Reset Service and Z-Controller (requires a connected BetaDisk interface)

**Configuration options:**
- Machine mode selection
- DivMMC On/Off (ZX Spectrum 128K / ZX Spectrum 48K / Timex modes)
- DivMMC / +3e MMC selection (ZX Spectrum +3 mode)
- TurboSound On/Off
- Kempston joystick interface On/Off

Configuration changes are applied directly to the CPLD and remain active until the device is powered off.

**Default power-on configuration:**
- Machine mode: ZX Spectrum 128K
- DivMMC: On
- TurboSound: On
- Kempston: On

---

## 🎮 How to Use

1. Power on the VSpider. The startup screen is displayed for approximately 1.5 seconds.
2. To enter the setup menu, hold down **CAPS SHIFT** while the startup screen is displayed.
3. Use **Q / A** to navigate through the menu options.
4. Press **SPACE / ENTER** to change the selected option.
5. Select **BOOT WITH THESE SETTINGS** and press **SPACE / ENTER** to apply the configuration and boot the machine.

**Additional information:**
- If **CAPS SHIFT** is not pressed, the machine boots automatically using the current CPLD configuration.
- The setup menu always starts with the default configuration values.
- Selecting ZX Spectrum +3 automatically selects +3e MMC.
- In Pentagon mode, disabling DivMMC makes the full 512 KB of RAM available.
- Selecting ZX Spectrum 128K or ZX Spectrum 48K automatically enables DivMMC.
- Configuration changes are not saved permanently and remain active only until the device is powered off.
- Timex-specific graphics modes (Hi-Res and Hi-Color) are available exclusively in Timex TC 2048 mode.
- The BetaDisk interface is supported in all non-Timex machine modes.

---

## 📝 Changelog

- **Rev. 1.5**
  - Added Gluk Reset Service (requires a connected BetaDisk interface).
  - Fixed several issues in Pentagon mode.
  - Z-Controller support has been restored.
  - Added the Pentagon 512 mode with Gluk Reset Service.

- **Rev. 1.4**
  - Fixed Pentagon timings.
  - In Pentagon mode, disabling DivMMC makes the full 512 KB of RAM available.
  - Fixed the BetaDisk interface. Again! ;-)
  - Partially implemented the floating bus.

- **Rev. 1.3**
  - Added Pentagon 128 machine mode.
  - Fixed a Kempston conflict with the BetaDisk interface.

- **Rev. 1.2**
  - Added Timex TC 2048 as a separate machine mode.
  - Timex-specific graphics modes (Hi-Res and Hi-Color) are now available exclusively in Timex TC 2048 mode and have been disabled in all other machine modes.
  - This change resolves a hardware conflict between Timex graphics modes and the BetaDisk interface, allowing BetaDisk to be used in all non-Timex machine modes.

- **Rev. 1.1**
  - Initial public release.

---

## 🔧 Hardware Configuration

The rightmost switch on the 3-position DIP switch forces ZX Spectrum 48K mode and disables the setup menu. This ensures compatibility with external interfaces, particularly disk interfaces.

---

## ⚠️ Known Issues

- If the SD card is not detected in +3e mode, press **RESET**.

---

## 🎥 Demo Video

[![YouTube](https://img.youtube.com/vi/bjnyU8IcQSs/0.jpg)](https://www.youtube.com/watch?v=bjnyU8IcQSs)