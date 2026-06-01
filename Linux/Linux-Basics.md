# Linux Basics

## What is Linux?

Linux is an open-source Unix-like operating system kernel created by Linus Torvalds in 1991. It powers servers, cloud platforms, containers, networking devices, and supercomputers worldwide.

## Why Linux for DevOps?

* Most cloud servers run Linux.
* Supports automation through shell scripting.
* Lightweight and highly customizable.
* Strong security and stability.
* Native support for DevOps tools.

## Linux Architecture

User
↓
Shell
↓
Kernel
↓
Hardware

### Components

1. Kernel

   * Core of Linux.
   * Manages CPU, memory, devices, and processes.

2. Shell

   * Command-line interpreter.
   * Examples: Bash, Zsh, Ksh.

3. File System

   * Organizes files and directories.

4. Utilities

   * Built-in tools such as ls, cp, mv, grep.

## Common Linux Distributions

| Distribution | Usage                 |
| ------------ | --------------------- |
| Ubuntu       | Cloud & Development   |
| CentOS       | Enterprise Servers    |
| RHEL         | Commercial Enterprise |
| Debian       | Stable Systems        |
| Amazon Linux | AWS Workloads         |

## Boot Process

1. BIOS/UEFI
2. Bootloader (GRUB)
3. Kernel Loading
4. Init/Systemd
5. Services Start
6. User Login

## Important Concepts

### Process

Running instance of a program.

Example:
ps -ef

### Service

Background application managed by systemd.

Example:
systemctl status sshd

### Package Manager

Ubuntu:
apt

RHEL/CentOS:
yum
dnf

## Hands-On Lab

1. Install Ubuntu VM.
2. Create user.
3. Install package.
4. Start service.
5. Create shell script.

## Interview Questions

Q: What is Linux?

A: Linux is an open-source Unix-like operating system kernel used in servers, cloud platforms, and enterprise environments.

Q: What is the difference between process and service?

A: A process is a running program, while a service runs continuously in the background.

Q: What is systemd?

A: systemd is the service manager responsible for booting and managing services.

## References

https://linuxjourney.com
https://ubuntu.com/tutorials
