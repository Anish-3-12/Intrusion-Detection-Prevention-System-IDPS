# 🛡️ Intrusion Detection and Prevention System (IDPS)

A lightweight Python-based IDPS that monitors system activity, detects potential intrusions based on predefined logic, and logs suspicious behavior in real-time. This tool is designed for educational or lightweight security purposes and demonstrates concepts in network and file system monitoring.

---

## 🧠 Features

- Monitors system and network activities
- Detects suspicious file access or unauthorized behaviors
- Logs all activity and detected intrusions
- Simple architecture, easy to extend and customize
- No heavy dependencies, runs on basic Python environment

---

## 📁 Project Structure

```
Intrusion-Detection-Prevention-System-main/
├── idps.py                      # Main script to run the IDPS
├── monitor.py                   # Monitoring logic (filesystem/network)
├── detector.py                  # Intrusion detection logic
├── requirements.txt             # Python dependencies
├── logs/
│   ├── file_log.txt             # Log of filesystem activity
│   └── network_connections_log.txt # Log of network activity
└── README.md
```

---

## ⚙️ Getting Started

### 1. Clone the Repository

```
git clone https://github.com/Anish-3-12/Intrusion-Detection-Prevention-System-IDPS.git
cd Intrusion-Detection-Prevention-System
```

### 2. Install Dependencies

```
pip install -r requirements.txt
```

### 3. Run the System

```
python idps.py
```

---
## Usage

- Edit the idps.py script and set the path variable to the directories you want to monitor.

- Run the IDPS: python idps.py

- The IDPS will begin monitoring the specified directory and the host system for any suspicious activity. Detected events will be logged in the following files:

1.file_system_log.txt: File system changes
2.network_connections_log.txt: Network connections
3.processes_log.txt: System processes

Additionally, the IDPS will alert the user if an anomaly is detected based on the number of events in a short period or unusual event patterns recognized by the Isolation Forest algorithm.

---

## 📑 Logs

All detected activity and potential intrusions are stored in the `logs/` directory:

- `file_log.txt`: Logs filesystem events
- `network_connections_log.txt`: Logs suspicious network connections

---

## 💡 Customization

- Modify `monitor.py` to add specific file/network rules.
- Update `detector.py` to enhance detection patterns (e.g., regex, thresholds).
- Extend functionality with notifications (email, SMS, etc.).

---

## 🙌 Final Note

This is a simplified educational implementation of an IDPS. For real-world use, consider industry-grade tools like Snort, Suricata, or OSSEC.

Contributions and suggestions are welcome. Stay safe! 🔐
