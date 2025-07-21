Project Overview

This project explores hands-on malware analysis and reverse engineering techniques using a fully Linux-based lab. It includes static analysis with tools like Ghidra, dynamic execution monitoring via `strace`, and custom rule creation with YARA. Optional components extend to Android malware and packed ELF binaries.



 Lab Environment

| Component | Purpose                  | OS       | Tools |
|----------|--------------------------|----------|-------|
| Kali     | Reverse engineering lab  | Kali     | Ghidra, Cutter, strace, ltrace, YARA, ClamAV |
| Ubuntu   | Log server + monitoring  | Ubuntu 24| Suricata, tcpdump, Wireshark               |

 Network Setup
- Isolated NAT or Host-Only Network**
- No Internet inside Kali VM (for safety)
- Snapshots enabled for VM rollback


Analysis Workflow

 Phase 1: Static Analysis
- Hash file (SHA256)
- Analyze with `strings`, `file`, `readelf`
- Load in Ghidra or Cutter
- Identify suspicious sections/functions

 Phase 2: Dynamic Behavior
- Monitor syscalls with `strace`, `ltrace`
- Network logs via `tcpdump`, `Wireshark`
- Check persistence mechanisms (e.g., crontab, .bashrc, systemd)

 Phase 3: Detection Rules
- Write YARA rule based on static features
- Scan sample set
- Test on variants

 Phase 4: Reverse Packed ELF
- Use UPX to pack a benign binary
- Unpack and reverse with Binwalk + Ghidra

 Bonus Phase: Android Reversing
- Tools: `apktool`, `jadx-gui`, `mobSF`
- Reverse permissions, smali code, manifest



 Tools Used
- Ghidra, Cutter (Radare2)
- strace, ltrace
- Wireshark, tcpdump, Suricata
- YARA, ClamAV
- apktool, jadx, MobSF (optional)
- UPX, Binwalk, Firmware-Mod-Kit (optional)

---

 Documentation
All analysis steps, findings, screenshots, and detection rules are documented in Medium blog series.



 Future Work
- Integrate Cuckoo Sandbox for full automation
- Add memory forensics using Volatility
- Try reversing IoT firmware



## 🔐 Disclaimer
This lab is for educational purposes **only**. Do not execute malware outside of an isolated environment.

---

Author
**Ibrahim Sheikh**  
[Medium](https://medium.com/@isheikh_24798) | [GitHub](https://github.com/IbraDevOps)


