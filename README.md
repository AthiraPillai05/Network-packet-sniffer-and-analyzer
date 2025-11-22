# Network-packet-sniffer-and-analyzer

A lightweight Python-based network packet sniffer that captures live traffic, analyzes anomalies, logs events, and provides an optional GUI for visualization.

✨ Features

Real-time packet sniffing (Scapy-based)

Logs traffic into SQLite database

Anomaly detection:

Port scans

Traffic spikes

Suspicious packet patterns

Alerting system (email/log-based)

GUI for live monitoring

📁 Project Structure
packetsniffer/
│── main.py          # Main entrypoint
│── sniffer.py       # Packet capture logic
│── analyzer.py      # Detection engine
│── alert.py         # Alert system
│── db.py            # SQLite wrapper
│── gui.py           # Optional GUI
│── packets.db       # Local SQLite database
│── alerts.log       # Alerts history

📦 Requirements

Install dependencies:

pip install scapy matplotlib yagmail


(Uses built-in sqlite3)

🚀 Usage
Run CLI Sniffer
sudo python main.py

Run GUI
sudo python gui.py

🛠 How It Works

sniffer.py captures packets

db.py stores metadata in SQLite

analyzer.py checks for anomalies

alert.py triggers logs/emails

gui.py visualizes traffic in real time

⚙️ Config (inside code)

You can adjust:

Interface

Thresholds

Email alert settings

Logging preferences

⚠️ Notes

Use only on networks you have permission to monitor

Requires root privileges (sudo)
