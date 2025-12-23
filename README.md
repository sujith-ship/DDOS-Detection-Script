Below is a **short, resume-friendly README.md**, including **attack simulation steps**, suitable for GitHub and concise enough for recruiters.

---

# DDoS Detection System (Libpcap)

A real-time **DDoS detection tool** built in **C using Libpcap** that monitors live network traffic and detects **TCP SYN, UDP, and ICMP flood attacks** using threshold-based analysis.

---

## Key Features

* Live packet capture on Linux
* Detection of SYN, UDP, and ICMP floods
* Source IP tracking for attack attribution
* Interval-based traffic analysis
* Lightweight and efficient implementation

---

## Tech Stack

* **C**, **Libpcap**
* **TCP/IP, UDP, ICMP**
* **Linux**

---

## How It Works

* Captures packets from a network interface
* Counts protocol-specific traffic per interval
* Triggers alerts when thresholds are exceeded
* Displays attack type, time, and top source IPs

---

## Setup & Run

```bash
sudo apt install libpcap-dev gcc
gcc ddos_detector.c -o ddos_detector -lpcap
sudo ./ddos_detector
```

(Update network interface in code if required.)

---

## Attack Simulation (Testing)

**TCP SYN Flood**

```bash
sudo hping3 -S --flood -p 80 <target-ip>
```

**UDP Flood**

```bash
sudo hping3 --udp --flood <target-ip>
```

**ICMP Flood**

```bash
sudo hping3 --icmp --flood <target-ip>
```

---

## Use Cases

* SOC monitoring
* Network security labs
* Cybersecurity projects
* Resume & academic demonstrations

---

## Author

**Tedlapu Sagar**
Cyber Security | Network Defense

---

If you want, I can also shorten this further to **3–4 lines for resume bullets** or add a **one-line GitHub description**.
