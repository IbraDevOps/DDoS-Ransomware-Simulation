DDoS & Ransomware Simulation Lab

This project demonstrates a simulated multi-stage cyberattack in a controlled virtual lab environment using Kali Linux and Ubuntu 17.10. It includes:

DDoS Attacks using tools like `ping`, `hping3`, and `nping`
Reverse Shell Access via Python script
Privilege Escalation Attempts using real kernel exploits (e.g., CVE-2017-5123)
Simulated Ransomware Behavior through GPG encryption and ransom notes

The objective is to understand how adversaries operate step-by-step — from initial access to impact — and to build awareness for blue teamers, students, and security professionals.

 Full walkthrough with screenshots, commands, and analysis available on Medium:
 [Read the article here](https://medium.com/p/10f7406cd668/edit)



 Lab Setup

Attacker VM: Kali Linux (192.168.1.30)
Victim VM: Ubuntu 17.10 (192.168.1.33)
Environment: VirtualBox with bridged networking

 Tools Used

 `hping3`, `nping` – traffic generation
 `python3`, `netcat` – shell interaction
 `gpg` – encryption
 `gcc` – exploit compilation

 Repo Contents

 `ransomware.md` – GPG encryption & ransom note simulation
 `PHP_reverse_shell` – Alt reverse shell
 `dirty.c`, `dirtycow.c` – Privilege escalation test code
 `Documentation.MD` – Full walkthrough steps



⚠️ Educational use only. Do not replicate outside of an isolated lab you own or control.
