# 🔐 Cisco Device Security Lab – Basic Configuration (Day 4)

This lab focuses on basic device security configuration for Cisco routers and switches using Cisco Packet Tracer. The tasks involve setting hostnames, securing privileged access, and saving configurations properly.
![image](https://github.com/user-attachments/assets/c5638d09-8a67-4e76-9afa-f1c5614ebf3a)

## 🧪 Lab Objectives

1. Change hostnames of both devices (e.g., `R1`, `SW1`) using global configuration mode.
2. Configure an unencrypted `enable password` (`CCNA`) on both devices.
3. Exit to user EXEC mode and test the password.
4. View the password in the running configuration.
5. Ensure all passwords are encrypted using the `service password-encryption` command.
6. View the encrypted password in the running config.
7. Replace the unencrypted password with an encrypted `enable secret` (`Cisco`).
8. Test access to privileged EXEC mode – determine which password is required.
9. Identify password encryption types:
   - **Type 7** → Weak encryption (used by `enable password`)
   - **Type 5** → MD5 encryption (used by `enable secret`)
10. Save the running configuration to the startup configuration (`copy running-config startup-config` or `write` command).

## 🛠️ Commands Used

```bash
hostname SW1
enable password CCNA
service password-encryption
enable secret Cisco
do show running-config
write memory
