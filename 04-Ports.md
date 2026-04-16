# 🔌 Ports (Network Ports)

## 🧠 What is a Port?

A **Port** is a logical number used to identify a specific service or process running on a server.

👉 It helps the server understand **which application should handle the request**

💥 **Key Idea:**  
👉 “IP tells WHERE, Port tells WHAT”

---

## 🏢 Real World Analogy

- IP Address = Building 🏢  
- Port = Room number 🚪  

👉 Example:

142.250.80.46:443


- 142.250.80.46 → Server (building)  
- 443 → HTTPS service (room)

---

## ❓ Why Ports are Needed?

👉 A single server can run multiple services:

- Website
- Database
- SSH
- Email

👉 Without ports:
❌ Server cannot differentiate requests

---

## 🔢 Port Range

| Range | Type |
|------|------|
| 0 – 1023 | Well-known ports |
| 1024 – 49151 | Registered ports |
| 49152 – 65535 | Dynamic / Ephemeral |

---

## 🔥 Common Ports (Important)

| Service | Port | Protocol |
|--------|------|----------|
| HTTP | 80 | TCP |
| HTTPS | 443 | TCP |
| SSH | 22 | TCP |
| FTP | 21 | TCP |
| MySQL | 3306 | TCP |

---

## 🌐 How Ports Work in Real Flow

When you open:

https://google.com


👉 Internally:


142.x.x.x:443


👉 Request goes to:
- IP → server
- Port → specific service (HTTPS)

---

## 📦 Packet Structure (With Port)

Each packet contains:


Source IP
Destination IP
Source Port
Destination Port
Data


👉 Example:


192.168.1.10:52345 → 142.x.x.x:443


- 52345 → client temporary port  
- 443 → server HTTPS port  

---

## 🔄 Source Port vs Destination Port

| Type | Meaning |
|------|--------|
| Source Port | Client side port (random) |
| Destination Port | Server service port |

---

## ⚡ Ephemeral Ports (Client Ports)

- Temporary ports used by client
- Range: 49152 – 65535
- Automatically assigned

👉 Used for:
- Browsing
- API calls

---

## 🔐 Port in HTTP vs HTTPS

| Protocol | Port |
|---------|------|
| HTTP | 80 |
| HTTPS | 443 |

👉 HTTPS uses encryption (TLS)

---

## 🧠 Behind the Scene

👉 When request reaches server:

- Server checks **destination port**
- Finds matching service
- Sends response

---

## 🛠️ Useful Commands (Linux)

Check open ports:

ss -tuln


Check processes using ports:

netstat -tulnp


---

## 📊 Summary

- Port identifies service
- Used with IP to route request
- Essential for multi-service servers
- Client uses temporary ports

---

## 💥 GOLD LINE

👉 “IP identifies the machine, Port identifies the service”