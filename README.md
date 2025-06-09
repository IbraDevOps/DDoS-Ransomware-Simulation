 DDoS & Ransomware Simulation Lab

This project simulates a basic DDoS attack and ransomware encryption scenario using two Kali Linux VMs in a bridged network setup.

 Network Setup
- Attacker VM: 192.168.1.30 (Kali)
- Victim VM: 192.168.1.33 

VMs are connected via VirtualBox bridged networking. Ping tests confirm stable communication.

 Simulation Phases
1. DDoS Attack using `hping3` from attacker to victim.
2. Ransomware Simulation by encrypting files with GPG on victim machine.
3. Decryption Process simulating ransom payment.

 Tools
- `hping3` – DDoS traffic simulation
- `gpg` – File encryption/decryption
- `bash` – Automation scripts
