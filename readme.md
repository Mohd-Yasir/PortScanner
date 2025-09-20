# Simple Python Port Scanner

This is a basic, multi-threaded port scanner built in Python. It's designed to be a learning tool to understand how network connections work and how to build ethical security tools.

## Features ✨

* **Fast Scanning**: Uses multi-threading to scan a large range of ports quickly.
* **Command-Line Interface**: Easy to use from the terminal with `argparse`.
* **Ethical Safety Check**: Includes a built-in warning for scanning public IP addresses.
* **User-Friendly Errors**: Provides clear error messages for common issues like permission denied.

## Prerequisites ⚙️

You only need Python 3 installed on your system.

## How to Use 🚀

1.  **Save the file**: Save the code as `scanner.py` on your computer.
2.  **Open your terminal**: Navigate to the directory where you saved the file.
3.  **Run the script**: Use the following commands to run the scanner.

**Basic Scan (default ports 1-100)**

```bash
python scanner.py localhost
Custom Port Range

Bash

python scanner.py localhost -p 80-81
Scanning a Public Host (Requires explicit 'yes' confirmation)

Bash

python scanner.py scanme.nmap.org -p 20-30
Interpreting Results 📊
[+] Port {port} is OPEN: A service is actively listening on this port.

[-] Port {port} is CLOSED: No service is listening on this port.

[!] Port {port} requires elevated permissions: Your user account does not have permission to access this port.

Ethical Disclaimer ⚖️
This tool is for educational purposes only. You should NEVER scan a network or host without having explicit, written permission from the owner. Unauthorized port scanning is illegal in many places. The creator of this tool is not responsible for any misuse.