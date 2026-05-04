# 🎯 IDOR

- **Platform:** TryHackMe
- **Difficulty:** Easy
- **Path:** Jr. Pen Testier
- **Objective:** Find and exploit IDOR vulnerabilities in a web application, giving unauthorized access.

---

## 🧠 Overview
IDOR is an access control vunerability, this room teaches about IDOR and how to exploit this vulnerability.

- IDOR stands for Insecure Direct Object Reference
- This vulnerability when exploited allows unauthorized access to objects
- <What skills are being taught>

---

## 🔍 Methodology

- <How tasks are organized>
- <How you approached solving them>
- <Any tools or mindset used>

---

## 📋 Tasks Breakdown

---

### ❓ Task 1 - What is an IDOR?
🥅 **Goal:**
- Defines what IDOR is and the importance of input validation.

🔑 **Key Takeaway:**
- IDOR is a type of vulnerability for that can occur when a web server receives user input to retrieve objects (files, data, documents).
- No validation on the server-side causes this vulnerability.
---

### 📝 Task 2 - An IDOR Example
🥅 **Goal:**
- Practice testing for IDOR vulnerability.

🛠️ **Approach:**
- Room gives a website that walks through an IDOR attack.

🔑 **Key Takeaway:**
- The way URL endpoints are structured can give hints to potential attack surfaces:
  i.e. /product/<number> => may be accessible to public/unauthorized users

---

### 🗺️🪪 Task 3 - Finding IDORS in Encoded IDs
🥅 **Goal:**
- To teach about encryption used through the web application and discovering IDORS with encoding throughout that web app.

🛠️ **Approach:**
- Explains that encryption is used in API post data, query strings or cookies.
- The room then shows an example of how a encoded string could be decoded to find a user ID.
- With that user ID the IDOR vulnerability is exploited.

🔑 **Key Takeaway:**
- Encoded data that is available to public presents an IDOR vulnerability
- Encoding can always be reversible
---

### 🗺️🪪 Task 4 - Finding IDORS in Hashed IDs
🥅 **Goal:**
- To teach about hashed IDS and how IDOR vulnerability is exploited.

🛠️ **Approach:**
- Explains its higher complexity vs. "encoding".
- The room shows how a web service might using hashing for IDs.
- With the use of open source tools to see if the hash can be "cracked".

🔑 **Key Takeaway:**
- Hashes are more secure than encoding techniques.
- Just as encoding it is still susceptible from "reversing", giving access to whatever encrypted data there is.
---

### 🗺️🪪 Task 5 - Finding IDORS in Unpredictable IDs
🥅 **Goal:**
- Explains the exploitation of using an ID of another user.

🛠️ **Approach:**
- Explains that if previous tasks are not "exploitable", try creating your own users and test it that way.

🔑 **Key Takeaway:**
- Users might be able to access another user's "data".
- "Brute Force" your way to finding an IDOR vulnerability, with multiple account creation and IDOR testing.
---

### 🤨 Task 6 - Where are IDORS locat
🥅 **Goal:**
- Explain where are IDORs can be located.

🔑 **Key Takeaway:**
- IDORS can be found in an address bar and elsewhere, like in an AJAX request.

---

### 🥋 Task 7 - A Practical IDOR Example
🥅 **Goal:**
- To practice what was learned from previous tasks.

🛠️ **Approach:**
- Utilizing a vulnerable machine given by Try Hack Me, the user tries to find IDORs.

🔑 **Key Takeaway:**
- <Lesson>
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