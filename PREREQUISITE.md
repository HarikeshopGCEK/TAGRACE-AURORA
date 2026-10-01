# 🏎️ IEEE ROBOCEK | TAG-RACE Workshop Prerequisites

Welcome to the **IEEE ROBOCEK TAG-RACE Workshop**!  
Please complete all the setup steps listed below on your laptop **before coming to the workshop** so you are ready to program and race your ESP32 car.

---

## 📋 Summary Checklist

- [ ] Installed **Arduino IDE** (v2.x recommended)
- [ ] Installed **CP210x USB Driver** (CP2102 / CP2104 VCP driver)
- [ ] Configured **ESP32 Board Manager URL** in Arduino IDE Preferences
- [ ] Installed **`esp32` Board Package** in Boards Manager
- [ ] Laptop charged & brought with **Data Cable** and **Power Adapter**

---

## 🛠️ Step-by-Step Installation Guide

### Step 1: Install Arduino IDE

1. Visit the official Arduino download page:  
   👉 **[https://www.arduino.cc/en/software](https://www.arduino.cc/en/software)**
2. Download and install **Arduino IDE 2.x** for your operating system (Windows / macOS / Linux).
3. Follow the installation wizard with default options.

---

### Step 2: Install CP210x USB Driver

The ESP32 microcontroller uses a CP2102 / CP210x USB-to-UART chip to communicate with your laptop over USB.

1. Download the driver from Silicon Labs:  
   👉 **[Silicon Labs CP210x VCP Drivers](https://www.silabs.com/software-and-tools/usb-to-uart-bridge-vcp-drivers?tab=downloads)** *(Download **CP210x Universal Windows Driver**)*
2. Extract the downloaded `.zip` file completely to a folder.
3. Install on **Windows**:
   - **Method 1 (INF File - Recommended):**  
     Inside the extracted folder, find **`silabser.inf`**, right-click it, and select **Install** (on Windows 11, click *Show more options* ➔ *Install*). Click **Yes** when Windows asks for permission.
   - **Method 2 (Batch File):**  
     Right-click **`update_param.bat`** and select **Run as Administrator**.
   - **Method 3 (Older `.exe` package):**  
     If your zip contains `CP210xVCPInstaller_x64.exe`, double-click and run it.
4. Install on **macOS**:
   - Open the downloaded `.dmg` package, run the installer, and allow security permissions under *System Settings > Privacy & Security*.
5. Restart your computer after installation if prompted.

---

### Step 3: Add ESP32 Board Manager URL

1. Open **Arduino IDE**.
2. Go to `File` ➔ `Preferences` (or `Arduino IDE` ➔ `Settings` on macOS / Keyboard shortcut `Ctrl + ,`).
3. Locate the **Additional boards manager URLs** field.
4. Paste the following URL into the box:

```text
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
```

*(If you already have another URL in that field, add a comma `,` at the end and paste this URL).*

5. Click **OK** to save.

---

### Step 4: Install ESP32 Board Package

1. In Arduino IDE, click on the **Boards Manager** icon on the left sidebar (or go to `Tools` ➔ `Board` ➔ `Boards Manager...`).
2. In the search bar, type `esp32`.
3. Locate **esp32 by Espressif Systems**.
4. Click **Install** (select the latest stable version).
5. Wait for the installation to finish (this may take a few minutes depending on your internet connection).

---

### Step 5: Test Board Selection

1. Connect your ESP32 board to your laptop using a USB data cable.
2. Go to `Tools` ➔ `Board` ➔ `esp32` ➔ select **DOIT ESP32 DEVKIT V1** (or **ESP32 Dev Module**).
3. Go to `Tools` ➔ `Port` and select the COM port corresponding to your connected ESP32 (e.g., `COM3`, `COM4` on Windows or `/dev/cu.usbserial-...` on Mac).

---

## 🎒 What to Bring to the Workshop

- [x] **Laptop** with all prerequisite software installed.
- [x] **Laptop Charger / Power Adapter**.
- [x] High enthusiasm for robotics & racing! 🚀

---

> 💡 **Need Help?** If you run into issues during setup, reach out to the **ROBOCEK** team or mentors before the workshop session.
