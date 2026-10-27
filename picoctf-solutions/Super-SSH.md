# 🌐 PicoCTF Challenge: Super SSH
* **Category:** General Skills
* **Points:** 25
* **Platform:** CyLab Security Academy / PicoCTF

---

## 📋 Challenge Description
The challenge requires us to connect to a secure remote server hosted by CyLab using an SSH connection credential and a specific port number.

## 🔍 Investigation & Logic
To securely control or inspect a remote machine over the internet, we cannot use basic browser tools. We must use **SSH (Secure Shell)**. 

To execute the connection properly, we must structure the command with the pattern: `ssh username@host -p port_number`. If we miss the `ssh` command prefix or fail to specify the designated port door (`-p`), the remote server will reject the handshake or give a `command not found` error.

## 🚀 Step-by-Step Solution
1. I clicked **Launch Instance** on the CyLab dashboard to spin up the target target machine.
2. I opened my local **Web Shell terminal**.
3. I initiated the secure connection using the following command string structure:
   ```bash
   ssh ctf-player@chatelaine.cylabacademy.net -p [YOUR_PORT_NUMBER]
   ```
4. I bypassed the security fingerprint prompt by typing `yes`.
5. I entered the temporary instance password provided by the platform (noting that the terminal completely hides the input visually for privacy safety).
6. Once logged into the remote environment, the machine instantly printed out my flag (academy{s3cur3_c0nn3ct10n_fbd97b2a})!

---

## 💡 Key Takeaways
* Mastered remote host authentication patterns utilizing the `ssh` protocol utility.
* Learned how to target specific listening application ports using the `-p` configuration flag.
* Understood that security terminal consoles purposely withhold masking indicators (`***`) during active password inputs.
