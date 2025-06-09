# DDoS-Ransomware-Simulation
This project simulates a basic DDoS attack and ransomware scenario using two Linux virtual machines.
#  DDoS and Ransomware Simulation Lab


- **Attacker VM:** 192.168.56.103
- **Victim VM:** 192.168.56.102

##  Communication
Ping test successful – VMs can reach each other via the host-only adapter.

##  Objectives
- Simulate a basic DDoS attack using `hping3`
- Simulate ransomware behavior using `gpg` to encrypt files
- Decrypt the files as if "ransom" was paid

##  Tools
- Kali Linux (both attacker & victim)
- hping3 (for DDoS)
- gpg (for encryption/decryption)
- bash scripts

##  Status
- [x] VM Setup
- [x] Network Configuration (Ping OK)
- [ ] DDoS Attack Simulation
- [ ] Ransomware Encryption
- [ ] Decryption Simulation
- [ ] Final Documentation & Demo

##  Next Step
Begin DDoS attack from attacker Kali (192.168.56.103) to victim Kali (192.168.56.102).
