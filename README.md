# 🔍 LAN Port Scanner

A lightweight LAN scanner written in Python, designed to identify open ports on devices within a local network using a simple external configuration file.

---

## 🎯 Project Objective

To enable fast, customizable, and multithreaded scanning of IP addresses in a local network, with the goal of:

- Detecting open ports
- Identifying active devices on the network
- Serving as a practical tool for learning internal network scanning

---

## ⚙️ How It Works

The script reads from a configuration file (`config.txt`) containing:

```
network=192.168.1.0/24
ports=22,80,443
```

It then:
1. Generates all possible IP addresses based on the subnet
2. Scans each specified port on each IP address
3. Displays the currently scanned address in real time
4. Presents a summary of all open ports found at the end
5. Shows the total runtime of the scan

---

## 🧪 Example Output

```
🔄 Currently scanning: 192.168.1.25:22
⚠️ 192.168.1.25   → OPEN PORTS: 22, 80
⚠️ 192.168.1.39   → OPEN PORTS: 443

✅ Scan complete in 12.84 seconds.
```

---

## 📁 Key Files

- `port_scanner_parallel.py` — main script file
- `config.txt` — configuration file (network address + ports)

---

## 🛠️ Requirements

- Python 3.6+
- No external dependencies (uses only built-in libraries)

---

## 📚 What I Learned

- Handling IP addressing and subnets
- Parsing configuration files
- Using Python sockets for port scanning
- Implementing multithreading with `ThreadPoolExecutor`
- Formatting and presenting data professionally

---

## 🧠 Personal Note

This project was built as part of my cybersecurity learning journey, through self-practice and full understanding of each component.  
It serves as a foundation for more advanced security tools I intend to develop.  
**This project was developed as part of hands-on cybersecurity practice, with a strong focus on understanding each component and its practical implications.
.**

---
