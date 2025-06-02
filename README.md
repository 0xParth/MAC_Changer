# MAC Changer 🔄

A Python script to temporarily change your MAC address for privacy and security testing.

## 🎯 Overview

MAC Changer is a simple yet powerful tool that allows you to change your network interface's MAC (Media Access Control) address. This can be useful for:
- Privacy protection on public networks
- Network security testing
- Bypassing MAC-based filters
- Development and testing purposes

## ✨ Features

- **Easy MAC Spoofing**: Change your MAC address with simple commands
- **Random MAC Generation**: Generate random valid MAC addresses
- **Vendor Preservation**: Option to keep the vendor prefix while randomizing
- **Restore Original**: Easy restoration of original MAC address
- **Cross-platform Support**: Works on Linux and macOS
- **Interface Selection**: Choose which network interface to modify

## 🔧 Prerequisites

- Python 3.x
- Root/sudo privileges
- Linux or macOS operating system
- `ifconfig` command available

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/0xParth/MAC_Changer.git
cd MAC_Changer

# Make the script executable
chmod +x MAC_IT.py
```

## 🚀 Usage

```bash
# Display help
sudo python MAC_IT.py --help

# Change MAC address to a specific value
sudo python MAC_IT.py -i eth0 -m 00:11:22:33:44:55

# Generate and set a random MAC address
sudo python MAC_IT.py -i wlan0 -r

# Show current MAC address
sudo python MAC_IT.py -i eth0 --show

# Reset to original MAC address
sudo python MAC_IT.py -i eth0 --reset
```

## 📋 Command Line Options

- `-i, --interface`: Network interface to change (e.g., eth0, wlan0)
- `-m, --mac`: New MAC address to set
- `-r, --random`: Generate and set a random MAC address
- `--show`: Display current MAC address
- `--reset`: Reset to original hardware MAC address
- `-h, --help`: Show help message

## 🔍 Examples

```bash
# Change MAC of WiFi interface to random address
sudo python MAC_IT.py -i wlan0 -r

# Set specific MAC address for Ethernet
sudo python MAC_IT.py -i eth0 -m aa:bb:cc:dd:ee:ff

# Check current MAC address
sudo python MAC_IT.py -i wlan0 --show
```

## ⚠️ Important Notes

- Changes are temporary and will reset after reboot
- Some network cards may not support MAC address changes
- Changing MAC address may temporarily disconnect your network
- Always ensure you have permission to change MAC addresses on the network

## 🛡️ Security Considerations

- Only use on networks you own or have permission to test
- Be aware of local laws regarding MAC address spoofing
- Some networks may detect and block spoofed MAC addresses

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License.

## ⚖️ Legal Disclaimer

This tool is for educational and authorized testing purposes only. Users are responsible for complying with applicable laws and regulations. The author is not responsible for any misuse or damage caused by this program.

## 👤 Author

**0xParth**
- GitHub: [@0xParth](https://github.com/0xParth)
- Twitter: [@0xparth](https://twitter.com/0xparth)
- Instagram: [@bug_xs](https://instagram.com/bug_xs)

## 🙏 Acknowledgments

- Inspired by the need for privacy in public networks
- Thanks to the Python community for excellent networking libraries
