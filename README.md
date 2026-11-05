# 🖨️ PrintCommand
### Your Complete Printer Troubleshooting & Command Reference Toolkit

<p align="center">
  <strong>Diagnose. Troubleshoot. Fix.</strong>
  <br>
  Discover useful printer commands, network diagnostics, Windows utilities, and troubleshooting solutions in one place.
</p>

<p align="center">
  <a href="https://printerhelpplus.com/">
    <img src="https://img.shields.io/badge/Printer%20Support-PrinterHelpPlus-1769AA?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Printer Help Plus">
  </a>
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Linux-blue?style=for-the-badge" alt="Platforms">
  <img src="https://img.shields.io/badge/Project-Open%20Source-16A6A0?style=for-the-badge" alt="Open Source">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License">
</p>

---

## 📌 About PrintCommand

**PrintCommand** is a printer troubleshooting and technical reference project designed to help users diagnose and resolve common printing problems using practical commands and step-by-step instructions.

From identifying network devices with `arp -a` to diagnosing connectivity issues, managing printer services, and troubleshooting stuck print jobs, PrintCommand brings useful technical resources together in one organized collection.

Whether you are a beginner, IT technician, system administrator, or printer support professional, this project aims to make printer troubleshooting easier and more accessible.

## ✨ Key Features

| Feature | Description |
|---|---|
| 💻 CMD Commands | Essential Windows Command Prompt commands |
| ⚡ PowerShell Utilities | Printer management and diagnostic commands |
| 🌐 Network Diagnostics | IP, ARP, DNS, ping, and connectivity tools |
| 🖨️ Printer Management | Manage printers, drivers, and printer ports |
| 🔧 Troubleshooting Guides | Practical solutions to common printer problems |
| 📋 Spooler Repair | Diagnose and resolve print queue issues |
| 📡 Network Printer Setup | Network printer configuration resources |
| 📚 Command Reference | Command syntax, explanations, and examples |

## 💻 Essential Troubleshooting Commands

### 1. Network Diagnostics

Useful commands for identifying network configuration and diagnosing printer connectivity.

| Command | Function |
|---|---|
| `arp -a` | Display IP-to-MAC address mappings |
| `ipconfig` | Display network configuration |
| `ipconfig /all` | Display detailed network information |
| `ipconfig /flushdns` | Clear the DNS resolver cache |
| `ping 192.168.1.100` | Test connectivity to a printer IP |
| `tracert 192.168.1.100` | Trace the network route |
| `nslookup google.com` | Perform a DNS lookup |
| `netstat -an` | Display network connections and listening ports |
| `getmac` | Display MAC addresses |
| `route print` | Display the routing table |

### 2. Windows Printer Management

Useful commands and utilities for accessing printer settings and managing installed printers.

| Command | Function |
|---|---|
| `control printers` | Open the Printers interface |
| `printmanagement.msc` | Open Print Management, if available |
| `services.msc` | Open Windows Services |
| `devmgmt.msc` | Open Device Manager |
| `printui /s /t2` | Open Print Server Properties and the Drivers tab |
| `Get-Printer` | List installed printers |
| `Get-PrinterDriver` | List installed printer drivers |
| `Get-PrinterPort` | List printer ports |
| `Get-PrintJob` | Retrieve printer jobs |

### 3. Print Spooler Troubleshooting

Restart the Windows Print Spooler service:

```cmd
net stop spooler
net start spooler
```

Check the Print Spooler service:

```cmd
sc query spooler
```

Clear stuck print jobs:

```cmd
net stop spooler
del /Q /F %systemroot%\System32\spool\PRINTERS\*.*
net start spooler
```

> ⚠️ **Important:** Clearing the spool directory deletes pending print jobs. Run these commands in an elevated Command Prompt.

### 4. PowerShell Diagnostics

```powershell
Get-Printer
Get-PrinterDriver
Get-PrinterPort
Get-PrintJob
Get-Service Spooler
Get-NetIPConfiguration
Get-NetAdapter
Test-NetConnection 192.168.1.100
```

These commands help inspect printer configurations, service status, and network connectivity.

## 🔧 Printer Troubleshooting Resources

PrintCommand covers common printer problems, including:

- 🖨️ Printer showing Offline
- 📄 Printer not printing
- 🔄 Print Spooler service errors
- 📋 Stuck or pending print jobs
- 🌐 Network printer connection issues
- ⚙️ Printer driver installation errors
- 📡 Wi-Fi printer connectivity problems
- 🧹 Paper jams and maintenance issues
- 🎨 Poor print quality
- 🔌 Printer not detected by Windows

## 🏷️ Supported Printer Brands

The documentation can include troubleshooting resources and setup instructions for popular printer manufacturers:

- HP
- Canon
- Epson
- Brother
- Xerox
- Ricoh
- Lexmark
- Kyocera

*PrintCommand is an independent resource and is not affiliated with these manufacturers.*

## 🛠️ Technology Stack

This project uses simple, accessible web technologies:

- HTML5
- CSS3
- Vanilla JavaScript
- Responsive Web Design
- GitHub Pages

No complex backend installation is required for the static website.

## 🚀 Getting Started

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to the project directory:

```bash
cd printcommand
```

Open `index.html` in your browser.

You can also use Visual Studio Code with the Live Server extension for local development.

## 📁 Project Structure

```text
PrintCommand/
│
├── index.html
├── commands.html
├── command.html
├── troubleshooting.html
├── network-tools.html
├── brands.html
│
├── tools/
│   ├── dpi-calculator.html
│   ├── paper-size-converter.html
│   └── print-cost-calculator.html
│
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
│
├── guides/
├── README.md
├── LICENSE
└── CONTRIBUTING.md
```

## 🌐 Need More Printer Support?

If you need more help with printer troubleshooting, installation, configuration, network connectivity, driver issues, or other printing-related problems, visit **[Printer Help Plus](https://printerhelpplus.com/)** for additional support and helpful resources.

## 🤝 Contributing

We welcome contributions from developers, IT professionals, and printer support enthusiasts.

You can contribute by:

- Adding useful CMD and PowerShell commands.
- Improving troubleshooting documentation.
- Adding printer setup tutorials.
- Correcting technical information.
- Improving website functionality.
- Reporting bugs and suggesting new features.

### Contribution Steps

1. Fork this repository.
2. Create a new feature branch.
3. Make your changes.
4. Commit your improvements.
5. Submit a Pull Request.

## ⚠️ Disclaimer

PrintCommand provides technical information and troubleshooting instructions for educational purposes.

Some commands require administrator privileges and may change system configurations or remove pending print jobs. Always review commands before executing them.

Driver downloads and manufacturer support resources should be obtained from official manufacturer websites.

PrintCommand and Printer Help Plus are independent resources and are not officially affiliated with HP, Canon, Epson, Brother, Xerox, Ricoh, or other printer manufacturers.

## 📄 License

This project is distributed under the MIT License. See the `LICENSE` file for details.

---


