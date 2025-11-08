# Project-PC-Music-Remote
Android music remote for PC — control desktop playback directly via Bluetooth(BLE ) or Wi-Fi.    
安卓音乐遥控器：通过蓝牙局域网直接控制电脑端音乐播放，

Control your PC music player directly via **Bluetooth Low Energy (BLE)**.  
Android acts as a remote controller, while the PC runs a BLE GATT service that wraps around VLC for playback control.

---

## ✨ Features
- Play / Pause / Next / Previous
- Volume control and position seek
- BLE pairing (secure, no internet)
- Real-time status feedback (Notify)
- VLC-based playback on desktop
- Planned dual-mode (BLE + Wi-Fi) in future branch

---

## 🧠 Architecture
| Component | Role | Tech Stack |
|------------|------|------------|
| **PC (Desktop)** | BLE GATT Server + VLC | Python 3.10+, Bleak, python-vlc |
| **Android (Client)** | BLE GATT Client (Control UI) | Kotlin, Jetpack Compose, BluetoothGatt |

Communication flow:

