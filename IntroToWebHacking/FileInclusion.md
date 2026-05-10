# 📁 File Inclusion

- **Platform:** TryHackMe
- **Difficulty:** Medium
- **Path:** Jr Penetration Tester
- **Objective:** Introduces file inclusion vulnerabilities, including LFI, RFI, and directory traversal.

---

## 🧠 Overview
Briefly describe what the room is about.

- <High-level concept 1>
- <High-level concept 2>
- <What skills are being taught>

---

## 🔍 Methodology
Describe HOW the room is structured and your approach.

- <How tasks are organized>
- <How you approached solving them>
- <Any tools or mindset used>

---

## 🧪 Key Concepts Covered

- Local File Inclusion (LFI)
- Remote File Inclusion (RFI)
- Directory Traversal
- Input validation weaknesses

---

### ℹ️ Task 1 - Introduction
🥅 **Goal:**
- To teach about File Inclusion and file inlcusion vulnerabilities.

🛠️ **Approach:**
- LFI, RFI and directory travel is introduced.
- Examples of File inclusion attacks are exploits are shown.

🔑 **Key Takeaway:**
- LFI = Local File Inclusion.
- RFI = Remote File Inclusion.
- Using query parameter strings you may be able to access files without authorization.
- Without proper input sanitiation an attacker may be able to write files into a server leading to a potential Remote Code Execution attacks.
---

### 🎰 Task 2 - Deploy the VM
🥅 **Goal:**
- Try Hack Me hosted vulnerable VM is powered on in this task.

---

### 🚶 Task 3 - Path Traversal
🥅 **Goal:**
- Directory Traversal is introduced in this task.
- Teaches multiple ways into acessing directories through poor input validation.

🛠️ **Approach:**
- THM educates the various ways an attacker can exploit path traversal vulnerabilities.
- THM teaches about very important directories a Linux + Windows machine have.
🔑 **Key Takeaway:**
- <Lesson>
- PHP code => file_get_contents
- Check for what the Operation System and type of device you are attacking. With that information you can attack file inclusion vulnerabilities using "input" based off of the machine you are attacking.
---

### 🗄️ Task 4 - Local File Inclusion
🥅 **Goal:**
- Teach about LFI attacks and importance of web app security when developing with PHP

🛠️ **Approach:**
- Room teaches about LFI and how programming languages present LFI vulnerabilities.
- Developer's need to be aware of certain LFI vulnerabilities.
- PHP is the language that this room presents LFI vulnerabilities.

🔑 **Key Takeaway:**
- Certain functions can give access to directories without proper input validation.
- Following code when entered into an HTTP request gives access to a different language directory.
```php
<?PHP
	include("languages/". $_GET['lang']);
?>
```
  - Using this code and manipulating it to access certain OS files allows for LFI/Path-traversal attacks
---

### 📁 Task 5 - LFI continued
🥅 **Goal:**
- Continuing with previous task, different LFI attacks are introduced in this task.

🛠️ **Approach:**
- 4 different ways an LFI attack can be made are shown.
- Knowledge of these 4 LFI attacks are applied through the Labs provided.

🔑 **Key Takeaway:**
- If your attack doesn't work in input, try putting the LFI attack throught he address bar.
- Directory traversal gives access to /etc directory; home of very important OS files
---

### 🕹️ Task 6 - Remote File Inclusion - RFI
🥅 **Goal:**
- To teach this technique to include remote files into a vulnerable application.

🛠️ **Approach:**
- Room educates how RFI attacks occur and explains consequences from RFI attacks.

🔑 **Key Takeaway:**
- RFI attacks can lead to Senstive Information Disclosure, Cross-Site-Scripting (XSS), Denial of Service (DoS).
- When there is no input validation, certain functions can allow malicious files to enter the web server from remote locations.
---

### 🏥 Task 7 - Remediation
🥅 **Goal:**
- This task lists common suggestions to prevent file inclusion vulnerabilities.

🔑 **Key Takeaway:**
- Keep web app frameworks updated.
- WAFs and proper input validation is important to prevent these attacks.

---

### 🚪 Task 8 - Challenge
🥅 **Goal:**
- To challenge the user to apply knowledge from room without help.

🛠️ **Approach:**
- Tests the knowledge of the user and applies knowledge from pre-requiste rooms.

🔑 **Key Takeaway:**
- Cookie tampering to exploit PHP include function.
- Post request
---

## 🧠 Lessons Learned

- <Big takeaway 1>
- <Big takeaway 2>
- <Big takeaway 3>

---



## 🚀 Improvements / Next Steps

- <What you would try next>
- <Tools you could add>
- <How to go deeper>

---

## 🔗 Room Link
<Insert TryHackMe link here>