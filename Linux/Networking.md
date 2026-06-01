# Networking.md

# Linux Networking

## Overview

Networking is a critical skill for DevOps Engineers because applications, servers, containers, and cloud services communicate through networks.

---

# OSI Model

| Layer | Name         | Example     |
| ----- | ------------ | ----------- |
| 7     | Application  | HTTP, HTTPS |
| 6     | Presentation | SSL/TLS     |
| 5     | Session      | NetBIOS     |
| 4     | Transport    | TCP, UDP    |
| 3     | Network      | IP          |
| 2     | Data Link    | Ethernet    |
| 1     | Physical     | Cable       |

---

# IP Address

Identify devices on a network.

Example:

192.168.1.10

Check IP Address:

```bash
ip addr
```

```bash
hostname -I
```

---

# Hostname

Check hostname:

```bash
hostname
```

Change hostname:

```bash
hostnamectl set-hostname devops-server
```

---

# DNS

DNS converts domain names into IP addresses.

Example:

google.com → 142.x.x.x

DNS Configuration:

```bash
cat /etc/resolv.conf
```

DNS Lookup:

```bash
nslookup google.com
```

```bash
dig google.com
```

---

# Routing Table

View routing table:

```bash
ip route
```

```bash
route -n
```

Example:

```bash
default via 192.168.1.1 dev eth0
```

---

# Network Interfaces

View interfaces:

```bash
ip link show
```

```bash
ifconfig
```

Bring interface up:

```bash
ip link set eth0 up
```

Bring interface down:

```bash
ip link set eth0 down
```

---

# Ping

Verify connectivity.

```bash
ping google.com
```

```bash
ping 8.8.8.8
```

---

# SSH

Remote server access.

Connect:

```bash
ssh user@server-ip
```

Generate Key:

```bash
ssh-keygen
```

Copy Key:

```bash
ssh-copy-id user@server-ip
```

---

# SCP

Secure file transfer.

Copy local file:

```bash
scp file.txt user@server:/tmp
```

Copy remote file:

```bash
scp user@server:/tmp/file.txt .
```

---

# Netstat

View network connections.

```bash
netstat -tulpn
```

Show listening ports:

```bash
netstat -an
```

---

# ss Command

Modern replacement for netstat.

```bash
ss -tulpn
```

```bash
ss -ant
```

---

# tcpdump

Capture packets.

Install:

```bash
sudo apt install tcpdump
```

Capture packets:

```bash
tcpdump -i eth0
```

Capture specific port:

```bash
tcpdump port 80
```

---

# Curl

Test APIs and websites.

```bash
curl google.com
```

```bash
curl -I google.com
```

---

# Wget

Download files.

```bash
wget https://example.com/file.zip
```

---

# Firewall

Check firewall:

```bash
ufw status
```

Allow SSH:

```bash
ufw allow 22
```

---

# Ports

| Port | Service     |
| ---- | ----------- |
| 22   | SSH         |
| 80   | HTTP        |
| 443  | HTTPS       |
| 3306 | MySQL       |
| 5432 | PostgreSQL  |
| 6379 | Redis       |
| 8080 | Application |

---

# Interview Questions

Q: Difference between TCP and UDP?

A: TCP is connection-oriented and reliable. UDP is connectionless and faster.

Q: What is DNS?

A: DNS translates domain names into IP addresses.

Q: What is SSH?

A: Secure protocol used to remotely access Linux servers.

Q: Which command checks open ports?

A: ss -tulpn or netstat -tulpn

---

# Hands-On Lab

1. Configure hostname.
2. Test DNS lookup.
3. Connect via SSH.
4. Capture packets using tcpdump.
5. Verify listening ports.
