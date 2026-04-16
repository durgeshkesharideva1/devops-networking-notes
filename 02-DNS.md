# 🌐 DNS (Domain Name System)

## 🧠 What is DNS?

DNS (Domain Name System) is a system that converts human-readable domain names into machine-readable IP addresses.

👉 Example:

google.com → 142.250.80.46


💥 **Key Idea:**  
👉 Humans use names, machines use IP addresses.

---

## ❓ Why DNS is Needed?

- Humans cannot remember IP addresses
- Websites are accessed using names (domains)
- DNS acts as a translator between name and IP

💥 **Line:**  
👉 “DNS = Internet ka Phonebook”

---

## 🔁 DNS Resolution Flow (Step-by-Step)

When a user enters a domain:


google.com


---

### 🟢 Step 1 — Browser Cache

- Browser checks if IP is already stored
- If found → request directly sent

---

### 🟢 Step 2 — OS Cache

- Operating system checks its DNS cache
- If found → use it

---

### 🟢 Step 3 — ISP DNS Resolver

- Request goes to ISP (Jio, Airtel etc.)
- If IP exists in cache → returned immediately

---

### 🔴 Step 4 — DNS Hierarchy (If not found)

#### 🔹 Root Server

- Top-level DNS server
- Does NOT give IP
- Provides direction to TLD

👉 Example:

.com server ke paas jao


---

#### 🔹 TLD Server (Top Level Domain)

- Handles domains like:
  - .com
  - .org
  - .in

- Does NOT give final IP
- Provides Authoritative server info

👉 Example:

google.com ke DNS server ke paas jao


---

#### 🔹 Authoritative Server

- Final source of truth
- Stores actual IP of domain

👉 Example:

google.com → 142.250.80.46


---

## 🔁 Complete Flow


Browser Cache
↓
OS Cache
↓
ISP DNS Resolver
↓
Root Server
↓
TLD Server
↓
Authoritative Server
↓
IP Address Found
↓
Back to Browser


---

## ⚡ DNS Caching (Important)

DNS results are stored temporarily.

### 📌 Why caching?
- Faster access
- Reduce load on DNS servers

---

## ⏳ TTL (Time To Live)

- Defines how long DNS record is stored
- After expiry → DNS lookup again

👉 Example:

TTL = 300 seconds


---

## 🌍 Types of DNS Records

### 🔹 A Record
Maps domain → IPv4


google.com → 142.x.x.x


---

### 🔹 AAAA Record
Maps domain → IPv6

---

### 🔹 CNAME
Maps domain → another domain

---

### 🔹 MX Record
Used for email servers

---

## 🧠 Real Life Analogy

👉 Searching address:

- Root → City office
- TLD → Area office
- Authoritative → Exact house

---

## 🔐 Security Note

- DNS itself is not encrypted
- Can be secured using:
  - DNS over HTTPS (DoH)
  - DNS over TLS (DoT)

---

## 📦 Summary

- DNS converts domain → IP
- Uses caching for speed
- Follows hierarchy:
  Root → TLD → Authoritative
- TTL controls cache duration

---

## 💥 GOLD LINE

👉 “DNS resolves domain using cache first, else hierarchical lookup”