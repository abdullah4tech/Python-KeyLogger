Keylogger 📜
Overview 📚
This repository provides a lightweight client-server keylogger architecture designed for educational purposes and authorized security auditing. It allows for real-time keystroke transmission from a target machine to a centralized monitoring server.

Warning: 🔒 Unauthorized use of keyloggers is illegal and unethical. Use this software only on systems where you have explicit, written permission.

Features 🌟
Dual-Logging: Keystrokes are stored locally in key_strokes.txt and transmitted via sockets.

Real-Time Monitoring: Live console output on the server-side as keys are pressed.

Network Capable: Supports remote monitoring over local networks or VPNs.

Minimal Footprint: Designed to run with basic Python dependencies.

Prerequisites 🛠️
Ensure the following are installed before running the scripts:

Python 3.x

pynput library (Install via: pip install pynput)

Usage 🚀
1. Server Setup
Run the server script on your monitoring machine to listen for incoming data:

Bash
python server.py
The server will initialize and wait for the client connection on the designated port.

2. Client Configuration
Open client.py and update the connection details:

Python
SERVER_IP = '127.0.0.1'  # Replace with your Server's IP address
PORT = 8080              # Ensure this matches the Server's port
Run the client on the target machine:

Bash
python client.py
3. Monitoring
The Server console will display real-time keystroke data.

The Client directory will generate a key_strokes.txt file containing the session log.

Ethical Usage & Legal Disclaimer ⚠️
This tool is provided strictly for educational and research purposes. The author assumes no liability for misuse or damage caused by this software.

Always respect privacy laws.

Obtain appropriate permissions before deployment.

Do not use for malicious data collection.

License 📝
This project is licensed under the MIT License.