````markdown
# 🔵 BlueConnect: Internet-Free Communication Tool

**BlueConnect** is an enterprise-grade peer-to-peer messaging application built in **Java** using the **BlueCove** library for Bluetooth communication. This tool enables users to discover nearby Bluetooth devices, establish RFCOMM connections, and exchange text messages **without the need for internet**.

---

## ✨ Features

- 🔍 Discover nearby Bluetooth devices  
- 🔗 Connect to selected device via Bluetooth RFCOMM  
- 💬 Real-time text messaging between paired devices  
- 🖥️ Clean and simple console interface (GUI version optional)  
- ♻️ Handles connection/disconnection gracefully  
- 🔐 *(Optional)* Basic message encryption for secure communication  
- 👥 *(Optional)* Support for multi-device group chat and file transfer

---

## 🤔 Why BlueConnect?

**BlueConnect** leverages Bluetooth’s **short-range wireless communication** to enable **offline messaging** in environments where internet access is unavailable or unreliable — such as:

- 🌍 Remote areas  
- 🎓 Classrooms or campuses  
- 🎪 Conferences or festivals  
- 🆘 Disaster zones

---

## ⚙️ Getting Started

### 🔧 Prerequisites

- Java Development Kit (JDK) 8 or higher  
- [BlueCove library](http://bluecove.org/)  
- Bluetooth-enabled hardware on both devices  
- OS: Windows or Linux (macOS has limited support)

---

### 🚀 Installation

1. **Clone this repository**:

   ```bash
   git clone https://github.com/yourusername/blueconnect.git
   cd blueconnect
````

2. **Download the BlueCove JAR** and add to your project:

   * [Download BlueCove](http://bluecove.org/download.html)
   * Place `bluecove-2.1.1.jar` in your project directory

3. **Compile Java files**:

   ```bash
   javac -cp bluecove-2.1.1.jar *.java
   ```

4. **Run the server**:

   ```bash
   java -cp .:bluecove-2.1.1.jar BluetoothServer
   ```

5. **Run the client** (replace MAC with server’s Bluetooth address):

   ```bash
   java -cp .:bluecove-2.1.1.jar BluetoothClient
   ```

---

## 🧪 Usage

* 🔹 Start the server on one device
* 🔹 Start the client on another device
* 🔹 Select server’s MAC address to connect
* 🔹 Type and send messages via the console
* 🔹 Watch real-time chat output

> ⚠️ GUI version (Swing/JavaFX) can be added as a future enhancement.

---

## 🗂️ Project Structure

```
blueconnect/
├── BluetoothServer.java       # Server-side messaging logic
├── BluetoothClient.java       # Client-side messaging logic
├── DeviceDiscoverer.java      # Utility for Bluetooth scanning
├── README.md                  # This file
├── bluecove-2.1.1.jar         # Bluetooth library (excluded from repo)
```

---

## 🚫 Limitations

* 📶 Bluetooth range is limited (~10 meters)
* 💻 Windows/Linux only (macOS has limited support)
* 🔐 No strong encryption (optional to add)
* 📡 One-to-one chat only (for now)

---

## 🔮 Future Improvements

* 🌐 Mesh networking for extended range
* 🖼️ GUI interface using Java Swing or JavaFX
* 📁 File transfer support
* 🔒 Message encryption & authentication
* 📥 Message queueing and auto-reconnect

---

## 🛠️ Troubleshooting

* ✅ Bluetooth must be ON for both devices
* ✅ Ensure proper drivers and permissions
* ✅ Try pairing devices via system settings if connection fails
* ✅ Check firewall/OS settings

---

## 🙏 Acknowledgments

* [BlueCove](http://bluecove.org/)
* Java Bluetooth (JSR-82) community
* Stack Overflow and open-source contributors ❤️

---

## 📄 License

This project is open-source under the **MIT License**.

---

## 📬 Contact

**Developer**: [Harsh Bhagat](mailto:harshbhagat9970.com)
**GitHub**: [Harsh Bhagat](https://github.com/harshbhagat22)

---

> 🛰️ *Stay connected, even offline — with **BlueConnect**!* 🔵

```

