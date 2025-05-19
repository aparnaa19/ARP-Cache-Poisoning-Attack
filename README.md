# ARP Cache Poisoning & MITM Lab (SEED Labs)

This project demonstrates ARP cache poisoning attacks using Scapy and Docker containers, and implements man-in-the-middle (MITM) attacks including Telnet and Netcat packet interception.

## 🔍 Objective
- Understand the ARP protocol and its vulnerabilities
- Launch ARP cache poisoning attacks using custom Python scripts
- Intercept and modify traffic between two victims (MITM)
- Use Scapy for crafting and sniffing ARP/TCP packets
- Perform packet rewriting for Telnet and Netcat traffic

## 🧰 Tools Used
- Docker (SEED Ubuntu VM)
- Scapy (Python)
- Wireshark
- Telnet
- Netcat

## 📌 Key Attack Scenarios
- **Simple ARP Poisoning:** Sent forged ARP replies to poison ARP caches
- **Gratuitous ARP:** Maintained poisoning state by repeatedly broadcasting spoofed ARP packets
- **MITM Attack (Telnet):** Replaced characters with 'Z' or 'A' in real-time using packet modification
- **Netcat Interception:** Demonstrated payload alteration in TCP stream between Host A and B

## 🛡️ Key Observations
- Poisoning was confirmed by checking ARP cache entries (`arp -n`)
- Telnet payloads were manipulated to show spoofed characters
- IP forwarding toggle was essential for controlling packet relay and interruption
- Packet sniffing validated attack success via Wireshark

## 🖼️ Screenshots
Optionally include screenshots of ARP cache, Wireshark captures, and spoofed Telnet messages.

## 📁 Files
- `arp-mitm-report.pdf` – Full documentation including code, steps, and observations

## 📄 Author
**Aparnaa Mahalaxmi Arulljothi**  
Student ID: A20560995

---

## 🔗 References
- [SEED Labs - ARP Cache Poisoning Lab](https://seedsecuritylabs.org/Labs_20.04/Networking/ARP_Attack/)
- [Scapy Docs](https://scapy.readthedocs.io/en/latest/)
