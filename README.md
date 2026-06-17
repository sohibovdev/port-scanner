# Local Port Scanner & Banner Grabber 📡

This project is a lightweight and fast port scanner written in Python, designed for local or remote network security auditing (pentesting) on Termux and Linux systems.

The tool scans the most commonly used network ports (such as SSH, FTP, HTTP, HTTPS, MySQL, etc.). If a port is open, it attempts to retrieve service/version information using Banner Grabbing techniques.

> ⚠️ **IMPORTANT:** This tool **DOES NOT REQUIRE ROOT PRIVILEGES**. It is 100% safe, stable, and works flawlessly on both Termux and Linux environments.

## ✨ Features
- 🚫 **No Root Required:** Runs perfectly without any administrator or superuser privileges.
- 🔍 **Banner Grabbing:** Attempts to grab banners to identify the software and versions running on open ports.
- ⚡ **Optimized Timeout:** Fast connection handling with a 1.0-second timeout per port to prevent hanging.
- 🎨 **Clean CLI Design:** Displays results in a clean, well-formatted, and color-coded table.

## 🛠️ Installation & Setup

The tool requires Python 3 and the `colorama` library for terminal text coloring.

### 1. Install Required Packages:
* **Linux (Ubuntu/Kali):**
  ```bash
  sudo apt update
  sudo apt install python3 python3-pip git -y
  ```
* **Termux:**
  ```bash
  pkg update
  pkg install python git -y
  ```

### 2. Clone the Repository & Install Dependencies:
```bash
git clone https://github.com
cd port-scanner
pip install colorama
```

## 🚀 How to Run
Run the tool using a standard user account:
```bash
python3 portscanner.py
```

## 📝 Usage Examples
Once the script starts, enter the target IP address or Domain Name:
- To scan your local device: `127.0.0.1`
- To scan your home Wi-Fi router: `192.168.1.1` (or `192.168.0.1`)
- To scan an external server: `example.com`
- 
