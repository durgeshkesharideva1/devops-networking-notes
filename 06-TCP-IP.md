# 🌐 TCP/IP (Transmission Control Protocol / Internet Protocol)

## 🧠 What is TCP/IP?

TCP/IP is a set of protocols used to send data over the internet.

- **IP (Internet Protocol)** → Identifies destination (address)
- **TCP (Transmission Control Protocol)** → Ensures reliable delivery

💥 **Key Idea:**  
👉 “IP tells WHERE, TCP ensures SAFE delivery”

---

## 🧩 TCP vs IP

| Protocol | Role |
|----------|------|
| IP | Addressing (where to send data) |
| TCP | Reliable delivery (how to send data) |

---

## 🔁 Complete Flow


Client → TCP Connection → Data Transfer → Server


---

## 🚀 TCP 3-Way Handshake

Before sending data, connection is established.

### 🔹 Step 1 — SYN
Client sends:
👉 “I want to connect”

---

### 🔹 Step 2 — SYN-ACK
Server replies:
👉 “Connection accepted”

---

### 🔹 Step 3 — ACK
Client confirms:
👉 “Let's start communication”

---

### 📊 Flow


Client → SYN
Server → SYN-ACK
Client → ACK


👉 Connection established ✔

---

## 📦 Packet Concept

Data is broken into small units called **packets**

---

## 🧠 Packet Structure

Each packet contains:


Source IP
Destination IP
Source Port
Destination Port
Sequence Number
Data


---

## 🔢 Sequence Number

- Helps maintain order
- Ensures correct data arrangement

---

## 🔁 Reliability (MOST IMPORTANT)

TCP ensures reliable delivery using:

---

### ✔ 1. Acknowledgement (ACK)

- Receiver confirms data received

---

### ✔ 2. Retransmission

- If packet lost → resend

---

### ✔ 3. Order Management

- Packets reassembled in correct order

---

### ✔ 4. Flow Control

- Prevents overwhelming receiver

---

## ⚡ Example Flow


Packet 1 → ACK ✔
Packet 2 → LOST ❌ → resend
Packet 3 → ACK ✔


---

## 🔄 Connection Termination

After communication ends:


FIN → ACK → FIN → ACK


👉 Connection closed

---

## 🔥 TCP vs UDP

| Feature | TCP | UDP |
|--------|-----|-----|
| Reliable | ✔ | ❌ |
| Fast | ❌ | ✔ |
| Use Case | Web, API | Streaming, Gaming |

---

## 🌐 Real World Mapping

- TCP = courier with tracking ✔
- UDP = normal post ❌

---

## 📦 Summary

- TCP ensures reliable communication
- Uses handshake to establish connection
- Data sent in packets
- ACK + retransmission ensures delivery

---

## 💥 GOLD LINE

👉 “TCP guarantees delivery, IP guarantees destination”