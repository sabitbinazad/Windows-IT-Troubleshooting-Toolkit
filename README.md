# Windows IT Troubleshooting Toolkit

A collection of PowerShell scripts and Windows utilities designed to help IT support technicians check hardware health, diagnose network connectivity, and troubleshoot common Windows system issues.

## Features

### 1. Disk Health Checker
- Detects physical disks recognized by Windows.
- Displays disk model, capacity, media type, and health status.
- Collects available temperature, wear, power-on hours, and read/write error information.
- Generates an HTML health report.

### 2. Battery Health Checker
- Generates a Windows battery report.
- Helps review battery capacity and battery wear.
- Saves the latest report in HTML format.

### 3. RAM Health Checker
- Displays installed memory modules, capacity, and speed.
- Shows current memory usage.
- Provides an option to launch Windows Memory Diagnostic.

### 4. CPU and Temperature Monitor
- Displays CPU model, core count, logical processors, and clock information.
- Shows CPU load information and processes using CPU resources.
- Checks for available Windows thermal-zone readings.
- Generates an HTML report.

### 5. Network and IT Troubleshooting
- Checks network adapters, IP addresses, and default gateway.
- Tests basic connectivity to the gateway and public IP addresses.
- Checks DNS resolution and selected TCP ports.
- Runs traceroute and displays the ARP cache.
- Shows active TCP connections.
- Generates an HTML diagnostic report.

## Requirements

- Windows 10 or Windows 11
- Windows PowerShell 5.1 or compatible PowerShell version
- Administrator permission may be required for some checks
- Network access for internet connectivity tests

Some hardware information depends on the device, driver, firmware, and Windows support.

## How to Use

1. Download or clone this repository.
2. Open the folder containing the desired tool.
3. Run the corresponding `.bat` launcher, if provided.
4. Approve the Windows User Account Control prompt when required.
5. Review the generated HTML report.

Keep each PowerShell script and its corresponding launcher in the same folder unless the script's instructions say otherwise.

## Reports

Reports are saved locally in the folders created by each tool. Filenames ending in `Latest.html` are overwritten when the tool runs again.

## Safety and Limitations

- These tools are intended for read-only diagnostics unless explicitly stated otherwise.
- They do not guarantee that hardware is free from faults.
- A failed ping does not necessarily mean a device is offline.
- Some disk health, SMART, and CPU temperature values may be unavailable on certain systems.
- Only run diagnostic checks on systems and networks you are authorized to troubleshoot.
- Back up important data regularly.

## Disclaimer

This project is provided for learning and IT troubleshooting purposes. Use it at your own discretion and verify important findings with official hardware diagnostics and Windows tools.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
