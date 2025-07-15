#  Build and Analyze a Custom Linux Rootkit in a Controlled Lab

This project explores the process of building, deploying, and detecting a simple Linux rootkit using Loadable Kernel Modules (LKMs) in a controlled, isolated lab environment. It's designed to push boundaries in kernel-level understanding, offensive security, and forensic detection.



 Full Walkthrough (with screenshots and step-by-step guide) is published on Medium:  
 [Read it here](https://medium.com/@yourusername/build-and-analyze-a-custom-linux-rootkit-in-a-controlled-lab-<article-slug>)  




 Project Goals

- Write a Loadable Kernel Module (LKM) that hides processes, files, and network ports.
- Simulate its deployment in a vulnerable Linux virtual machine.
- Detect and analyze its behavior using real-world forensic and monitoring tools.
- Document both offensive techniques and defensive detection strategies.

---

 Lab Setup

- Target VM: Ubuntu 18.04 / 20.04 (64-bit)
- Attacker/Monitor VM: Kali Linux
- Tools Used:
  - `gcc`, `insmod`, `rmmod`, `lsmod`, `dmesg`
  - `ps`, `top`, `netstat`, `lsof`, `/proc`
  - `chkrootkit`, `rkhunter`, `Volatility`, `Syscall diffing`




 ⚠️ Disclaimer

This project is **for educational use only**. Do **NOT** deploy or test this code outside of an isolated lab environment. Misuse of rootkits in production or public environments may be illegal and unethical.

---

Author

Ibrahim Sheikh  
Cloud Security & Offensive Security Enthusiast  
 GitHub: [@IbraDevOps](https://github.com/IbraDevOps)  
 Medium: [@isheikh_24798](https://medium.com/@isheikh_24798)



