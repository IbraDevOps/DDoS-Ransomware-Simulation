##  DDoS Attack Simulation (hping3)

- **Attacker IP:** 192.168.1.30
- **Victim IP:** 192.168.1.33
- **Tool Used:** hping3

Command used:

```bash
sudo hping3 --flood -S -p 80 192.168.1.33

Port 80 was chosen after running a basic HTTP server on the victim.

The attack caused high SYN traffic, simulating a DoS scenario.
