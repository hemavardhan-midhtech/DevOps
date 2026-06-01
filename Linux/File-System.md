# Linux File System

## Overview

Linux uses a hierarchical file system starting from the root directory (/).

## Directory Structure

## Directory Structure 
/
├── bin
├── boot
├── dev
├── etc
├── home
├── lib
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin
├── srv
├── sys
├── tmp
├── usr
└── var


## Important Directories

### /etc

Configuration files.

Examples:

/etc/passwd
/etc/hosts
/etc/fstab

### /var

Variable data.

Examples:

/var/log
/var/spool

### /home

User home directories.

Example:

/home/devops

### /tmp

Temporary files.

### /proc

Kernel and process information.

## File Types

| Symbol | Type             |
| ------ | ---------------- |
| -      | Regular File     |
| d      | Directory        |
| l      | Symbolic Link    |
| c      | Character Device |
| b      | Block Device     |

Example:

ls -l

## Permissions

r = Read = 4

w = Write = 2

x = Execute = 1

Example:

-rwxr-xr--

755

Owner = rwx

Group = r-x

Others = r-x

## Hard Link vs Soft Link

Hard Link

ln file1 file2

Soft Link

ln -s file1 file2

## Disk Usage Commands

df -h

du -sh *

lsblk

fdisk -l

## Interview Questions

Q: What is inode?

A: Metadata structure storing file information except filename.

Q: Difference between hard link and soft link?

A: Hard links share inode; soft links point to another file path.

Q: Which directory stores logs?

A: /var/log

## Lab

1. Create directory structure.
2. Create symbolic link.
3. Change permissions.
4. Check disk usage.
