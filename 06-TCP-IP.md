# 🌐 HTTP & HTTPS (Web Communication)

## 🧠 What is HTTP?

HTTP (HyperText Transfer Protocol) is a protocol used for communication between client (browser) and server.

👉 It defines how requests are sent and responses are received.

💥 **Key Idea:**  
👉 “HTTP defines WHAT client wants from server”

---

## 🔁 Basic Flow


Client → HTTP Request → Server
Server → HTTP Response → Client


---

## 📤 HTTP Request

A request sent by client to server.

### 🧪 Example:

GET / HTTP/1.1
Host: google.com


---

## 🧠 Request Breakdown

### 🔹 1. Method
Defines action:

| Method | Meaning |
|--------|--------|
| GET | Fetch data |
| POST | Send data |
| PUT | Update data |
| DELETE | Remove data |

---

### 🔹 2. Path

/ → homepage
/login → login page


---

### 🔹 3. HTTP Version

HTTP/1.1


---

### 🔹 4. Headers

Extra information sent with request.

### 🧪 Example:

Host: google.com
User-Agent: Chrome
Accept: text/html


👉 **Host = which website**
👉 **User-Agent = which browser**
👉 **Accept = what type of data**

---

### 🔹 5. Body (POST only)

Used to send data:


username=durgesh
password=123


---

## 📥 HTTP Response

Server reply to client.

### 🧪 Example:

HTTP/1.1 200 OK


---

## 📊 Status Codes

### 🟢 2xx (Success)
- 200 OK

### 🔴 4xx (Client Error)
- 404 Not Found

### 🔥 5xx (Server Error)
- 500 Internal Server Error

---

## 🔐 What is HTTPS?

HTTPS = HTTP + TLS (Security Layer)

👉 Data is encrypted before sending

---

## 🔒 Why HTTPS?

- Protects data
- Prevents hacking
- Ensures secure communication

---

## 🔁 HTTPS Flow


Client → TLS Handshake → Secure Connection
↓
HTTP Request (Encrypted)
↓
Server Response (Encrypted)


---

## 🔐 TLS (Transport Layer Security)

- Encrypts communication
- Uses certificate for identity

---

## 📜 Certificate

Server identity proof.

Contains:
- Domain name
- Public key
- Issuer (CA)

---

## 🧠 HTTP vs HTTPS

| Feature | HTTP | HTTPS |
|--------|------|-------|
| Security | ❌ No | ✔ Yes |
| Encryption | ❌ | ✔ |
| Port | 80 | 443 |

---

## 🌐 Real Flow Example


https://google.com

↓
DNS → IP
↓
TCP connection
↓
TLS handshake
↓
HTTP request (encrypted)
↓
Server response
↓
Browser renders page


---

## 📦 Summary

- HTTP = communication protocol
- HTTPS = secure HTTP
- Uses request & response model
- Status codes define result

---

## 💥 GOLD LINE

👉 “HTTP tells what you want, HTTPS protects it”