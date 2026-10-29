# 🤖 CyLab Challenge: Trust But Verify
* **Category:** Artificial Intelligence / Easy
* **Points:** 30
* **Platform:** CyLab Security Academy

---

## 📋 Challenge Description
An interactive ethics and technical puzzle designed to teach the critical hazards of unverified AI outputs. The goal is to act as an auditor, cross-examining AI-generated claims and scripts to find hidden bugs and discrepancies.

## 🔍 Investigation & Logic
Because the `nc` (Netcat) utility captures the entire primary terminal stream to display the interactive narrative, local testing cannot happen in the same prompt. 

To audit the AI's claims, I opened a split-terminal panel workspace. While the game prompt ran on the left, I utilized the right-hand environment to manually run `ls` and `cat` against the files the AI claimed to have processed. This allowed me to catch where the AI hallucinated structural code logic versus the physical facts on the disk.

## 🚀 Step-by-Step Solution
1. Launched the instance on the CyLab dashboard.
2. Opened the terminal workspace and initiated the interactive socket stream using Netcat:
   ```bash
   nc xebec.cylabacademy.net 39269
   ```
3. Advanced through the scenario text by pressing `Enter`.
4. When the AI presented its programmatic assertions, I opened a secondary terminal tab to inspect the actual system script.
5. By auditing the real file, I discovered the discrepancy, answered the interactive prompts with the correct verified evidence, and completed the scenario layout.
6. **Final Flag Extracted:** `academy{7ru57_15_34rn3d_a5b4c2e0}`

---

## 💡 Key Takeaways
* **Verify Everything:** AI systems write code with absolute confidence but are highly prone to subtle logic omissions and hallucinations.
* **Workspace Management:** Mastered 