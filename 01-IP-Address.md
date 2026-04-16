# 📍 IP Address (Internet Protocol)

## 🧠 What is an IP Address?

An **IP Address** is a unique identifier assigned to every device connected to a network.

It is used to identify and communicate between devices over the internet.

👉 Example:

142.250.80.46


💥 **Key Idea:**  
👉 IP tells **WHERE** to send the data.

---

## 🌍 Types of IP Address

### 🔹 1. Public IP
- Used on the internet
- Assigned by ISP (Internet Service Provider)
- Unique globally

👉 Example:

142.250.x.x


---

### 🔹 2. Private IP
- Used inside local network (LAN)
- Not visible on internet
- Assigned by router (DHCP)

👉 Example ranges:

10.0.0.0 – 10.255.255.255
172.16.0.0 – 172.31.255.255
192.168.0.0 – 192.168.255.255


---

## 🧠 IPv4 Structure

An IPv4 address consists of **32 bits**, divided into 4 parts:


192.168.1.1


Each part = 8 bits (1 byte)

---

## 📊 CIDR Notation

CIDR defines how many bits are used for network.

👉 Example:

192.168.1.0/24


- 24 bits = network
- 8 bits = host

---

## 🔢 Number of IPs

👉 Formula:

2^(32 - CIDR)


👉 Example:

/24 → 2^(32-24) = 256 IPs


---

## 🔁 DHCP (Dynamic IP Assignment)

DHCP automatically assigns IP to devices.

👉 Flow:
1. Device connects to network  
2. DHCP server assigns IP  
3. Device uses it temporarily  

---

## 🔄 NAT (Network Address Translation)

NAT converts:

Private IP → Public IP


👉 Why?
- Save IP addresses  
- Allow multiple devices to share one public IP  

---

## 🌐 Real Flow


Laptop (192.168.x.x)
↓
Router (NAT)
↓
Public IP (Internet)
↓
Server (142.x.x.x)


---

## 📦 Summary

- IP = Unique address of device  
- Private IP = Local network  
- Public IP = Internet  
- DHCP = Assigns IP  
- NAT = Converts IP  

---

## 💥 GOLD LINE

👉 **“IP tells WHERE, NAT connects LOCAL to INTERNET”**