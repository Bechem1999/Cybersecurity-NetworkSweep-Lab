# Cybersecurity-NetworkSweep-Lab
# Network Device Sweep & Intrusion Detection Lab

## 📌 Lab Title
Network Sweep Script Development using Bash (Kali Linux)

---

## 🎯 Objective

The objective of this lab was to:

1. Create a group called security.
2. Add at least 3 users to the group (e.g., alice_sec, bob_sec,
carol_sec).
3. Ensure only members of the security group can execute the sweep
script.
4. Create a script named testsweep.sh
5. The script should:
- Accept a subnet as an argument (e.g., 192.168.15).
- Sweep from .1 to .254 using ping.
- Capture the response and extract IP addresses.
- Write results to a file named sweep_results.txt.

---

## 🛠 Tools Used

- Kali Linux
- Bash Scripting
- ping (ICMP)
- Linux Networking Commands
- GitHub

---

## 📝 Step-by-Step Process

1. Created a security group
2. Created three groups and added the three users to the security group
3. created a script named "testsweep.sh"
4. Ensured only members of the security group can execute the sweep script by setting the correct permissions using the command " chmod u+x testsweep.sh`
5. Added argument validation for subnet input
6. Implemented a loop to sweep IP range (1–254)
7. Used ping with timeout control to test host availability
8. Captured successful responses
9. Logged active IPs into `sweep_results.txt`
10. Made the script executable using `chmod u+x`
11. Executed the script against target subnet

---

## 💻 Commands Executed

- sudo groupadd Security
- getent group security
- sudo useradd -m alice_sec
- sudo useradd -m bob_sec
- sudo useradd -m carol_sec
- sudo mkdir -p /home/shared/security
- sudo chown :security testsweep.sh
- sudo chmod 750 tetsweep.sh
- ls -alps
- chmod u+x testsweep.sh
- cat testsweep.sh
- cat sweep_results.txt
- ls -l /home/shared/security/testsweep.sh
- mousepad testsweep.sh


## Key Observations / Lessons Learned

- Subnet accuracy is critical when performing network scans.
- Bash scripting is powerful for automation in cybersecurity investigations.
- Logging and structured output improve incident documentation.

.

🚀 Skills Demonstrated

- Network reconnaissance fundamentals
- Bash scripting automation
- Troubleshooting network connectivity
- Linux command-line proficiency
- Documentation and professional GitHub presentation
