# xLogger 🕵️‍♂️

**xLogger** is a lightweight, stealth-oriented keystroke monitoring tool built with Python. It combines background monitoring with a secure user access layer and a real-time visualization interface.

The application is designed to be completely invisible during operation, accessible only through a hidden system tray icon after a successful secure login.

---

## 🌟 Key Features

* **🛡️ Secure Authentication**: A built-in Login & Registration system using **SHA-256 password hashing**. No plain-text passwords are ever stored.
* **👻 Stealth Operation**: Once logged in, the application window disappears from the taskbar and runs exclusively in the **System Tray**.
* **⚡ Real-Time Feed**: A dedicated GUI window (hidden by default) that displays live keystrokes in a clean, terminal-style interface.
* **🧹 Smart Logging**: Automatically filters "junk" characters and control keys. It handles backspaces in the log file using a `*` notation for easy readability.
* **🔒 Single Instance Lock**: Uses socket-binding logic to ensure only one instance of `xLogger` runs at a time, preventing duplicate logs and system lag.
* **📦 Standalone Executable**: Fully compatible with PyInstaller for conversion into a single `.exe` file.

---

## 🛠️ Tech Stack

| Component | Library/Module |
| :--- | :--- |
| **GUI** | Tkinter |
| **Input Capture** | `pynput` |
| **System Tray** | `pystray` & `Pillow` |
| **Security** | `hashlib` |
| **Process Control** | `socket` & `threading` |

---

## 🚀 Installation & Setup

### 1. Prerequisites
Ensure you have Python 3.x installed. You will need to install the following dependencies:

```bash
pip install pynput pystray Pillow
