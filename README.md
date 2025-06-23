# cybersecurity-task1
# Network Reconnaissance with Nmap and Wireshark

![Nmap Logo](https://nmap.org/images/sitelogo.png)

A demonstration of basic network scanning techniques using Nmap to identify active hosts and open ports on a local network.

## Project Overview

This repository contains results from a TCP SYN scan (`-sS`) performed on a local network (192.168.37.0/24) using Nmap on Kali Linux. 

## Scan Details

**Command Used:**
```bash
sudo nmap -sS 192.168.37.0/24 -oN scan_results.txt
sudo wireshark
