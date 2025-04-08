# SniffChat 🛜🔍

**SniffChat** is a simple network tool that combines:
- 🛜 **UDP-based chat system** with optional encryption.
- 🔍 **Packet sniffer** that captures and analyzes network packets like Wireshark.
- 🗂️ **Packet saving** feature to `.pcap` files for later analysis.

Built in **Python**, without using `tcpdump` or external sniffers.

---

## ✨ Features

- **UDP Chat**
  - Connect to an IP and Port.
  - Send and receive encrypted or plain messages.
- **Packet Sniffer**
  - Capture Ethernet, IP, and UDP packets.
  - Parse and display packet information.
  - Apply filters (capture only certain IPs/ports).
- **Save Packets**
  - Save captured packets to `.pcap` files.
- **Statistics**
  - View number of packets captured and total bytes.
- **Error Handling**
  - Robust against malformed or corrupted packets.
- **Clean Output**
  - Color-coded, readable console output.

---

## 📦 Project Structure

```bash
SniffChat/
├── main.py          # Entry point for chat and sniffer
├── sniffer.py       # Sniffer logic (capture, parse, save packets)
├── chat.py          # Chat logic (send, receive, encrypt messages)
├── pcap_writer.py   # Functions for creating .pcap files
├── utils.py         # Utilities (encryption, packet parsing helpers)
