
# 💬 Chat Room with Server — Python TCP Project

This project is a simple **multi-client chat room** built in **Python** using **TCP sockets** and a **Tkinter GUI**.  
It allows multiple users (clients) to chat with each other in real-time through a central server.

---

## 🧠 What This Project Does

- Enables **real-time text chat** between multiple users.  
- Uses **socket programming** for client–server communication.  
- Runs on a **single computer (localhost)** or across a **LAN network**.  
- Uses **multithreading** so multiple users can chat simultaneously.  
- Includes a **Tkinter GUI** for clients — making it easy and user-friendly.

---

## ⚙️ Technologies Used

| Component | Description |
|------------|-------------|
| **Language** | Python 3.x |
| **Networking** | TCP/IP sockets |
| **Concurrency** | Threading |
| **GUI Framework** | Tkinter |

✅ All these modules are part of **Python’s standard library** — no extra installation is required.

---

## 📦 Files Included

Server_TCP.py # The server script — handles clients and message broadcasting
├── Client.py # The client GUI application


---

## 🧰 Requirements

Before running this project, make sure you have:
- **Python 3.8** or newer installed  
- A working terminal (Command Prompt, VS Code terminal, etc.)

You can verify Python installation using:
```bash
python --version


How to Run the Project

python Server_TCP.py
python Client.py
Step 3 — Start Chatting

Type your message in the input box and click Send.

The message will appear in all connected client windows.

The server terminal shows all incoming messages and connections.


💬 Example Output
Server Terminal:
Server listening on 127.0.0.1:5050
Client connected: 127.0.0.1:50124
Client connected: 127.0.0.1:50125
127.0.0.1:50124: Hello everyone!
127.0.0.1:50125: Hi there!


Client Window:
Welcome to the Chat Room!
127.0.0.1:50124: Hello everyone!
127.0.0.1:50125: Hi there!


How It Works
The server script starts a TCP socket on an IP and port.

Each time a client connects, the server creates a new thread to handle it.

When any client sends a message, the server broadcasts it to all connected clients.

The Tkinter GUI displays all messages in real time.
