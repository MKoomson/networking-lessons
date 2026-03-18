# Networking Lesson – Subnetting & HTTP/HTTPS Basics

## 🧠 Subnetting Fundamentals

Subnetting is the process of dividing a network into smaller networks (subnets) for better organization and security.

### Key Concepts:

* **Subnet Mask** determines the size of each subnet
* **CIDR Notation** (e.g., /26, /27, /28) defines how many bits are used for the network
* **Block Size Formula:**
  `256 - subnet mask value = subnet increment`

### Examples:

* /26 → block size = 64 → subnets: 0, 64, 128, 192
* /27 → block size = 32 → subnets: 0, 32, 64, 96…
* /28 → block size = 16 → subnets: 0, 16, 32, 48…

### Important Addresses:

* **Network Address** → first IP in subnet
* **Broadcast Address** → last IP in subnet
* **Usable Range** → everything in between

---

## 🌐 Public vs Private Subnets (Cloud Concept)

In real-world cloud environments:

* **Public Subnet**

  * Contains resources accessible from the internet
  * Example: Web servers

* **Private Subnet**

  * Contains resources not directly accessible from the internet
  * Example: Databases

### Basic Architecture:

* Internet → Public Subnet (Web Server)
* Web Server → Private Subnet (Database)

---

## 🔐 HTTP vs HTTPS

### HTTP (HyperText Transfer Protocol)

* Data is sent in **plain text**
* Not secure
* Vulnerable to interception

### HTTPS (HyperText Transfer Protocol Secure)

* Data is **encrypted**
* Uses SSL/TLS for security
* Protects sensitive information (passwords, user data)

### Key Difference:

* HTTP → readable data ❌
* HTTPS → encrypted data ✅

---

## 🔑 Key Insight

Security in modern systems comes from combining:

* **Network Design (subnets)**
* **Protocol Security (HTTPS)**

---

## 🚀 What I Learned Today

* How to calculate subnet ranges and identify network/broadcast addresses
* How subnetting applies in real cloud environments
* The difference between HTTP and HTTPS
* How secure architecture separates public and private resources

---

## 📌 Next Steps

* Deep dive into how HTTPS works (SSL/TLS basics)
* Learn how cloud platforms implement networking (AWS VPC, subnets)
* Continue building real-world scenarios

---
