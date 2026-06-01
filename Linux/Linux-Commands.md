# Linux-Commands.md

# Essential Linux Commands for DevOps

## Navigation

```bash
pwd
ls
ls -la
cd
tree
```

## File Operations

```bash
touch file.txt
cp file1 file2
mv file1 file2
rm file.txt
rm -rf folder
```

## Directory Operations

```bash
mkdir project
mkdir -p app/logs
rmdir folder
```

## File Viewing

```bash
cat file
less file
more file
head file
tail file
tail -f file
```

## Search

```bash
find / -name file.txt
locate nginx
which python
whereis nginx
```

## Text Processing

```bash
grep error logfile
grep -i warning file
awk '{print $1}'
sed 's/dev/prod/g'
cut -d':' -f1
sort
uniq
wc -l
```

## Compression

```bash
tar -cvf backup.tar files
tar -xvf backup.tar
gzip file
gunzip file.gz
zip file.zip file
unzip file.zip
```

## User Management

```bash
useradd john
passwd john
usermod
userdel
groupadd devops
groups
id
```

## Permissions

```bash
chmod 755 file
chmod 644 file
chown user:user file
chgrp group file
```

## Process Management

```bash
ps -ef
top
htop
pgrep nginx
pkill nginx
kill PID
kill -9 PID
```

## Service Management

```bash
systemctl start nginx
systemctl stop nginx
systemctl restart nginx
systemctl status nginx
systemctl enable nginx
```

## Networking

```bash
ping google.com
ssh user@server
scp file server:/tmp
curl localhost
wget url
```

## Network Analysis

```bash
ip addr
ip route
ss -tulpn
netstat -tulpn
tcpdump
dig google.com
nslookup google.com
```

## Disk Management

```bash
df -h
du -sh *
lsblk
fdisk -l
mount
umount
```

## Memory Monitoring

```bash
free -h
vmstat
sar
```

## CPU Monitoring

```bash
top
htop
mpstat
lscpu
```

## Logs

```bash
journalctl
tail -f /var/log/syslog
dmesg
```

## Package Management (Ubuntu)

```bash
apt update
apt upgrade
apt install nginx
apt remove nginx
```

## Package Management (RHEL)

```bash
yum install nginx
yum update
dnf install nginx
```

## Environment Variables

```bash
env
printenv
export JAVA_HOME=/opt/java
```

## Scheduling Jobs

```bash
crontab -e
crontab -l
```

Cron Example:

```bash
0 2 * * * /opt/backup.sh
```

## Shell Scripting

```bash
#!/bin/bash
echo "Hello DevOps"
```

Run Script:

```bash
chmod +x script.sh
./script.sh
```

## Useful One-Liners

Top CPU Processes:

```bash
ps aux --sort=-%cpu | head
```

Top Memory Processes:

```bash
ps aux --sort=-%mem | head
```

Largest Directories:

```bash
du -sh * | sort -hr
```

Find Large Files:

```bash
find / -type f -size +1G
```

Open Ports:

```bash
ss -tulpn
```

---

# Top 20 Commands Every DevOps Engineer Must Know

1. ls
2. cd
3. pwd
4. grep
5. find
6. cat
7. tail
8. chmod
9. chown
10. ps
11. top
12. systemctl
13. journalctl
14. ssh
15. scp
16. curl
17. df
18. du
19. ip
20. ss

---

# Interview Tip

Master these commands without notes:

* grep
* find
* awk
* sed
* systemctl
* journalctl
* ssh
* curl
* df
* du
* top
* ps

These commands alone cover nearly 70% of Linux-related DevOps interview questions.
