# 🛡️ Wireshark Revision Guide

Wireshark is a powerful network protocol analyzer that captures and inspects packets in real time. It’s widely used in cybersecurity for troubleshooting, traffic analysis, and identifying potential attacks. This guide serves as a quick reference for revisiting key concepts and workflows.

---

## 📖 **Core Concepts**

- **Packet**: Small unit of data transmitted over a network.
- **Frame**: Data link layer encapsulation of packets.
- **Protocol Layers**:
  - Layer 2 (Data Link): Ethernet, ARP
  - Layer 3 (Network): IP, ICMP
  - Layer 4 (Transport): TCP, UDP
  - Layer 7 (Application): HTTP, DNS, FTP

- **Capture Filters vs. Display Filters**:
  - 📥 **Capture Filters**: Set **before** capturing packets.
    - Example: `tcp port 80`
  - 🔍 **Display Filters**: Apply **after** capturing packets.
    - Example: `http.request.method == "GET"`

---

## ⚡ **Essential Filters**

| **Type**           | **Filter Syntax**               | **Description**                      |
|---------------------|-----------------------------------|----------------------------------------|
| IP Traffic          | `ip.addr == 192.168.1.5`        | All traffic to/from IP                |
| Subnet Traffic      | `ip.addr == 192.168.1.0/24`     | Filter subnet                         |
| Protocol Specific   | `http`                          | Only HTTP packets                     |
| Source IP           | `ip.src == 10.0.0.2`            | Packets sent **from** IP              |
| Destination Port    | `tcp.dstport == 443`            | Packets sent **to** port 443          |
| TCP Handshake       | `tcp.flags.syn == 1`            | SYN packets (start of handshake)      |
| DNS Queries         | `dns.qry.name == "example.com"` | DNS query for domain                  |

---

## 🧠 **Key Features**

- 🕵️ **Follow TCP Stream**  
  Reconstructs a full conversation between two hosts.

- 📄 **Packet Details Pane**  
  Expands headers (Ethernet, IP, TCP/UDP, Application).

- 🛡️ **Color Coding**  
  - Black: Errors
  - Green: TCP traffic
  - Light Blue: DNS traffic

- 🗺️ **GeoIP**  
  Map IPs to countries (requires GeoIP DB).

---

## 🛠️ **Practical Use Cases**

- 🔎 **Identify Open Ports**: Look for SYN-ACK responses in TCP handshakes.  
- 🌐 **Analyze HTTP Requests**: Find GET/POST parameters.  
- 🚨 **Detect Attacks**:
  - ARP Spoofing: Duplicate IPs in ARP replies.
  - DNS Tunneling: Unusually long DNS queries.
  - DoS: Excessive SYN packets (SYN flood).  

---

## 🎯 **TryHackMe Challenges Completed**
- ✅ **Carnage Room**: Practiced packet filtering, HTTP analysis, and reconstructing credentials from traffic captures.

---

## ⚡ **Quick Tips**
- 🏃 Start capturing: `Ctrl+E`
- 🛑 Stop capturing: `Ctrl+E` again
- 🔖 Bookmark packets: Right-click → "Mark Packet"
- 💾 Export filtered packets: File → Export Specified Packets

---


📌 *Always capture traffic ethically and with permission.*
