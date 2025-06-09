##  DDoS Attack Simulation (hping3)

- **Attacker IP:** 192.168.1.30
- **Victim IP:** 192.168.1.33
- **Tool Used:** hping3

Command used:

```bash
sudo hping3 --flood -S -p 80 192.168.1.33

Port 80 was chosen after running a basic HTTP server on the victim.

The attack caused high SYN traffic, simulating a DoS scenario.


To simulate remote attacker access in a real-world compromise, a PHP reverse shell was used to gain a foothold on the victim machine (192.168.1.33) from the attacker's machine (192.168.1.30).

 Why PHP Reverse Shell?
Many web servers run Apache/Nginx + PHP.

PHP reverse shells are lightweight, simple to deploy, and effective in bypassing basic defenses.

Useful in scenarios where file upload vulnerabilities or command injection allow the attacker to execute arbitrary code on the web server.
