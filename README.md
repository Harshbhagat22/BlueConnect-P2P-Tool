# BlueConnect: Internet-Free Communication Tool

**BlueConnect** is an enterprise-grade peer-to-peer messaging application built in **Java** using the **BlueCove** library for Bluetooth communication. This tool enables users to discover nearby Bluetooth devices, establish RFCOMM connections, and exchange text messages **without the need for internet**.

---

## Features

- Discover nearby Bluetooth devices  
- Connect to selected device via Bluetooth RFCOMM  
- Real-time text messaging between paired devices  
- Clean and simple console/GUI-based chat interface  
- Handles connection/disconnection gracefully  
- (Optional) Basic message encryption for secure communication  
- (Optional) Support for multi-device group chat and file transfer

---

## Why BlueConnect?

BlueConnect leverages Bluetooth’s **short-range wireless communication** protocol to enable **offline messaging** in environments where internet access is unavailable or unreliable — such as remote areas, conferences, festivals, or disaster zones.

---

## Getting Started

### Prerequisites

- Java Development Kit (JDK) 8 or higher  
- [BlueCove library](http://bluecove.org/) (Bluetooth Java library)  
- Bluetooth-enabled hardware on both devices  
- Compatible OS (Windows, Linux; macOS support limited)  

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/blueconnect.git
   cd blueconnect
````

2. Download the BlueCove JAR and add it to your project’s classpath:

   * Download: [http://bluecove.org/download.html](http://bluecove.org/download.html)
   * Place `bluecove-2.1.1.jar` in your project directory

3. Compile the Java files (example for command line):

   ```bash
   javac -cp bluecove-2.1.1.jar *.java
   ```

4. Run the server:

   ```bash
   java -cp .:bluecove-2.1.1.jar BluetoothServer
   ```

5. Run the client on another device (replace MAC with server’s address):

   ```bash
   java -cp .:bluecove-2.1.1.jar BluetoothClient
   ```

---

## Usage

* Start the server application on one device.
* Start the client application on the other device, connecting to the server’s Bluetooth address.
* Exchange messages via the console input/output.
* Type messages and press Enter to send.

---

## Project Structure

```
blueconnect/
├── BluetoothServer.java       # Server program for Bluetooth messaging
├── BluetoothClient.java       # Client program to connect and chat
├── DeviceDiscoverer.java      # Device scanning and discovery utility
├── README.md                 # This file
├── bluecove-2.1.1.jar        # BlueCove Bluetooth library (not included in repo)
```

---

## Limitations

* Bluetooth range is limited (~10 meters).
* Works best with Bluetooth-enabled devices on Windows/Linux.
* macOS support for BlueCove is limited and may require additional setup.
* No advanced encryption or authentication implemented (can be added).

---

## Future Improvements

* Implement mesh networking for extended range
* Add GUI for better user experience
* Support file transfer and group chat
* Add message encryption and authentication
* Implement reconnection and message queueing

---

## Troubleshooting

* Make sure Bluetooth is enabled on both devices
* Verify device compatibility with BlueCove
* Run with appropriate permissions (especially on Linux)
* Check firewall or OS Bluetooth settings if connection fails

---

## Acknowledgments

* [BlueCove](http://bluecove.org/) for the Bluetooth Java API
* Java Bluetooth Specification (JSR-82) for guidance
* Community forums and tutorials for Bluetooth socket programming

---

## License

This project is open source under the MIT License.

---

## Contact

For questions or feedback, reach out to:

* Your Name — [Harsh Bhagat](mailto:harshbhagat9970.com)
* GitHub: [Harsh Bhagat](https://github.com/harshbhagat22)

---

*Stay connected, even offline — with BlueConnect!* 🚀
