# 🐧 My Personal Linux & Cybersecurity Tips

This is my living cheat sheet for quick commands, syntax shortcuts, and handy tips I discover while practicing.

---

### 🔍 File Inspection Tips
* `cat [filename]` — Opens and reads the entire content of a file on your screen instantly.
* `strings [filename]` — **Tip:** If a file looks like unreadable computer gibberish, this command extracts only the readable English text inside it! (Great for finding hidden flags).

### 🗺️ Navigation Shortcuts
* `ls` — Lists all files in your current folder.
* `cd ..` — **Tip:** Type this to move backward exactly one folder (like hitting the "Back" button on your browser).
* `clear` — Wipes the terminal screen clean if it gets too cluttered with text.

### Challenge Shortcuts Learnt 
1st Challenge: To find a Flag in a file link
clear (to clear the screen)
wget http:// (put the download file link here)
ls (to see the files in the folder)
cat flag (to get the flag from the file).

2nd Challenge: Connecting to a secure server 
This is an SSH (Secure Shell)
Click Lunch Instance (the remote server)
Copy the Remote Server Credentials 
Paste it in your terminal and hit enter like this: ssh ctf-player@chatelaine.cylabacademy.net -p 38865
Select Yes for connection prompt 
Copy password from the hint given 
Paste password in terminal and hit enter
Now you're in 
ls (to see the files in the server folder)
cat the file name (to read the Flag).

---
*💡 Rule of thumb: If I have to look up a command twice, it belongs on this list!*
