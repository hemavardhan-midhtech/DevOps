# Troubleshooting.md

# Linux Troubleshooting Guide

## Overview

Troubleshooting is one of the most important DevOps skills. The goal is to quickly identify, isolate, and resolve issues.

---

# System Information

```bash
uname -a
```

```bash
hostnamectl
```

```bash
uptime
```

---

# CPU Troubleshooting

CPU Usage:

```bash
top
```

```bash
htop
```

```bash
mpstat
```

High CPU Processes:

```bash
ps aux --sort=-%cpu
```

---

# Memory Troubleshooting

Check Memory:

```bash
free -h
```

```bash
vmstat
```

Top Memory Consumers:

```bash
ps aux --sort=-%mem
```

---

# Disk Troubleshooting

Disk Space:

```bash
df -h
```

Large Directories:

```bash
du -sh *
```

Largest Files:

```bash
find / -type f -size +500M
```

---

# Process Troubleshooting

List Processes:

```bash
ps -ef
```

Search Process:

```bash
ps -ef | grep nginx
```

Kill Process:

```bash
kill PID
```

Force Kill:

```bash
kill -9 PID
```

---

# Service Troubleshooting

Check Status:

```bash
systemctl status nginx
```

Start Service:

```bash
systemctl start nginx
```

Restart Service:

```bash
systemctl restart nginx
```

Enable Service:

```bash
systemctl enable nginx
```

---

# Log Analysis

System Logs:

```bash
journalctl
```

Recent Logs:

```bash
journalctl -xe
```

Follow Logs:

```bash
tail -f /var/log/messages
```

```bash
tail -f /var/log/syslog
```

---

# Network Troubleshooting

Check Connectivity:

```bash
ping google.com
```

Check Routes:

```bash
ip route
```

DNS Test:

```bash
dig google.com
```

Open Ports:

```bash
ss -tulpn
```

---

# Storage Troubleshooting

Check Block Devices:

```bash
lsblk
```

Disk Details:

```bash
fdisk -l
```

Mount Information:

```bash
mount
```

---

# File Permission Issues

View Permissions:

```bash
ls -l
```

Change Permissions:

```bash
chmod 755 file.sh
```

Change Ownership:

```bash
chown user:user file.sh
```

---

# Performance Analysis

Load Average:

```bash
uptime
```

IO Analysis:

```bash
iostat
```

```bash
iotop
```

---

# Troubleshooting Workflow

1. Identify issue.
2. Gather logs.
3. Check service status.
4. Verify resources.
5. Verify network.
6. Implement fix.
7. Validate solution.
8. Document findings.

---

# Common DevOps Issues

## Application Not Accessible

Check:

```bash
systemctl status
```

```bash
ss -tulpn
```

```bash
curl localhost
```

## Disk Full

```bash
df -h
```

```bash
du -sh *
```

## Server Slow

```bash
top
```

```bash
free -h
```

```bash
iostat
```

---

# Interview Questions

Q: How do you troubleshoot high CPU?

A: Use top, htop, ps aux and identify the consuming process.

Q: How do you troubleshoot a service failure?

A: Check systemctl status, logs, resource usage, and dependencies.

Q: How do you troubleshoot disk space issues?

A: Use df -h and du -sh to locate large files/directories.

---

# Hands-On Lab

1. Simulate CPU stress.
2. Fill disk space.
3. Stop a service.
4. Analyze logs.
5. Recover service.
