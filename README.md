# 🔥 ARP-Spoofer — Multi-Target ARP Poisoning Tool (Python 2 & Scapy)

A lightweight ARP spoofing (ARP poisoning) tool written in **Python 2** using **Scapy**.  
This script performs ARP poisoning between **multiple pairs of hosts**, allowing you to place yourself in a Man‑in‑the‑Middle (MITM) position for **ethical hacking labs**.

> ⚠️ Use only on networks you own or have explicit permission to test.

---

## 🚀 Features

- Works on **Python 2** (compatible with Python 3 with minor edits)
- Spoofs ARP tables of **three IP addresses** (Router ↔ Host1, Router ↔ Host2, Host1 ↔ Host2)
- Can be used with **any devices** (Windows, Linux, VMs, physical machines, etc.)
- Automatically restores original MAC addresses on exit (CTRL + C)
- Real‑time packet counter
- Clean and simple Scapy implementation

---

## 📦 Requirements

Install Scapy for Python 2:

```bash
pip install scapy

On Kali Linux (Python 2 environment):
➡️sudo apt-get install python-scapy
🛠 Usage
➡️sudo python arp_spoofer.py -i <IP1> -w <IP2> -m <IP3>

Example
If you have:
Router: 10.168.1.1
Windows VM: 10.168.1.10
Metasploit VM: 10.168.1.12
➡️sudo python arp_spoofer.py -i 10.168.1.1 -w 10.168.1.10 -m 10.168.1.12

📂 Project Structure:
ARP-Spoofer/
│── arp_spoofer.py
└── README.md

⚠️ Legal & Ethical Notice
This tool is intended only for:
Ethical hacking labs
Cybersecurity study
Virtual machine testing environments
Penetration tests with written permission

Unauthorized MITM attacks are illegal.
Use responsibly.




