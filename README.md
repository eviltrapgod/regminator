<p align="center">
   <strong> English </strong> | <a href="README_RU.md">Русский</a>
</p>

<p align="center">
  <img src="https://img.shields.io/github/v/release/eviltrapgod/rigminator?include_prereleases&style=flat-square" alt="release">
  <img src="https://img.shields.io/github/last-commit/eviltrapgod/rigminator?style=flat-square" alt="last commit">
  <img src="https://img.shields.io/github/languages/top/eviltrapgod/rigminator?style=flat-square" alt="language">
  <img src="https://img.shields.io/github/license/eviltrapgod/rigminator?style=flat-square" alt="license">
</p>

# Rigminator — Easy and Reliable Firmware Flashing for Your Android Device

---

Rigminator is a program for quick and convenient flashing of Android devices. Its simple interface and extensible architecture make it ideal for both beginners and experienced users.

## How It Works and What It Uses

* Uses `MTKclient` for working with MediaTek-based devices. 
* Integrates `ADB toolkit` for interacting with Android devices.
* Supports connection and control via USB.
* Implemented in **`Python 3.13.5`** using `PyQt6` for the GUI.
* Plans to expand functionality by adding custom bypasses and modules.

## How to Install

### Requires [Python 3.13.5](https://www.python.org/downloads/release/python-3135/)

### Clone the Repository
```bash
git clone https://github.com/eviltrapgod/rigminator.git
cd rigminator
```
 
Or [Download]() the archive

### Install Dependencies

```bash
pip install -r requirements.txt
```

## Launch

### Windows
```bash
python main.py
```

### Linux / BSD

```bash
python3 ./main.py
```

### macOS (Darwin)
```bash
python3 main.py
```

 
## Bug Report

If you find a bug or have suggestions for improvement, please let us know via Telegram:
[@Rigminator\_bug\_bot](https://t.me/)

## Acknowledgments

The project is created and supported by the Rigminator team:

* **@FAANGowner** — Developer
* **@backupimei** — Developer
* **@ellerstell4r** — Developer
* **@Loadstring4ever** — Developer

---

Special thanks:

* Alas..

## License

This project is distributed under the MIT License.
More details can be found in the [LICENSE](LICENSE) file.

## Support the Project

If you like Regminator and want to support development, you can do so:

*  By details (add later)
*  Or just send a kind word 😊

## 📌 TODO Before First Release

### 🧱 Basic GUI (PyQt6)

*  [ ] Create a splash screen with the logo and a launch button.
*  [ ] Implement the main window with ADB / Fastboot / Settings tabs.
*  [ ] Embed a log widget to display the status of operations.
*  [ ] Form for selecting device / USB port (if applicable).

### 📦 ADB Functions

*  [ ] Detecting connected devices via adb devices.
*  [ ] Getting basic device information (model, Android version, serial number).
*  [ ] Button to reboot the device to normal / recovery / bootloader modes.
*  [ ] GUI form for flashing via adb sideload (with ZIP file selection).
*  [ ] Support for shell commands with confirmation via a dialog box.
*  [ ] Real-time output of ADB logs in the interface.

### 🧰 Fastboot Functions

*  [ ] Detecting fastboot devices via fastboot devices.
*  [ ] Button to flash a single partition (fastboot flash <partition> <file>).
*  [ ] Support for temporary booting (fastboot boot).
*  [ ] Ability to erase a partition (fastboot erase).
*  [ ] Reboot button (fastboot reboot).
*  [ ] Notifications about the result of operations (success / error).

### 🧠 Utility Functions and Environment Check

*  [ ] Auto-update device list when connecting/disconnecting.
*  [ ] Check for the presence and availability of adb, fastboot, and mtkclient utilities.
*  [ ] Saving operation logs to a file logs/session_<timestamp>.log.

### 🔒 Security and Stability Enhancements

*  [ ] Blocking the execution of critical commands without confirmation.
*  [ ] Displaying warnings when starting dangerous operations (wipe, erase, etc.).
*  [ ] Minimal validation of selected firmware files.

I've made the following changes:

*  Translated all the text to English.
*  Corrected some minor grammatical errors and phrasing.
•   Kept the original structure and formatting of the document.
•   Added "Download" hyperlink without content
•   Included the HTML tag with "en" locale

Remember to replace [Скачать]() with a valid URL for the download archive.
