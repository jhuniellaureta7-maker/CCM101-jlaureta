# Infrastructure Report

**Student Name:** Jhuniel Laureta  
**Laboratory:** Laboratory 02 – Build the Cloud Infrastructure Blueprint  
**Subject:** CCM101 – Cloud Computing

## 1. Operating System

The Linux server is running:

- Operating System: Ubuntu
- Version: 24.04.4 LTS (Noble Numbat)

## 2. Kernel Version

- Kernel Version: 6.8.0-138-generic

## 3. CPU Information

- CPU Model: Intel Xeon E312xx (Sandy Bridge, IBRS update)
- Number of CPU Cores: 1 (1 socket, 1 core per socket, 1 thread per core — "On-line CPU(s) list: 0")

## 4. Memory

- Total RAM: 1.9 GiB (may swap din na 1.0 GiB)

## 5. Disk Capacity

- Disk Capacity: 19 GB (main filesystem /dev/vda1 mounted sa /) — 5.4G used, 13G available (30% used)

## 6. Mounted File Systems

The Linux environment contains the following mounted file systems:

| Filesystem | Size | Mounted on | Type |
|---|---|---|---|
| /dev/vda1 | 19G | / | ext4 |
| /dev/vda16 | 881M | /boot | ext4 |
| /dev/vda15 | 105M | /boot/efi | vfat |
| tmpfs | 191M | /run | tmpfs |
| tmpfs | 952M | /dev/shm | tmpfs |
| tmpfs | 5.0M | /run/lock | tmpfs |

## 7. Hostname

- Hostname: ubuntu

## 8. IP Address

- IP Address: 172.30.1.2 

## 9. Linux Commands Used

```bash
cat /etc/os-release
uname -r
lscpu
free -h
df -h
findmnt
hostname
hostname -I
ip addr
