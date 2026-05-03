# ❌ Authentication Bypass
- Platform: TryHackMe
- Difficulty: Easy
- Objective: Learn how to defeat logins and other authentication mechanisms to allow you access to unpermitted areas.
- Path: Jr. Penetration Tester

## 🧠 Overview
- This room demonstrates various attack surfaces that can be exploited on authentication mechanisms.
  
## 🔍 Methodology
- Each task teaches different ways authentication mechanisms can be attacked, then demonstrates how those vulnerabilities are exploited. 
- The user applies this knowledge by completing practical exercises and answering questions based on each exploitation scenario.
--------
### 🩲 Task 1 - Brief
- Setup for Room; Start Machine is done
--------
### 👤 Task 2 - Username Enumeration
🥅 Goal:
- Discover usernames with ffuf tool

🔑 Key Takeway:
- When signing up for a website there usually is text that is sent to the website which indicates the username is being used.
- Use that text to find usernames being used

--------
### 🦍 Task 3 - Brute Force
🥅 Goal:
- Find the username/password combo with ffuf

🔑 Key Takeway:
- Utilize wordlists with usernames discovered and brute force login with passwords
--------
### 🤔📈 Task 4 - Logic Flaw
🥅 Goal:
- To teach about poor design in "logical paths" in authentication mechanisms

🔑 Key Takeway:
- Logical flaws can exist in any area of a website

--------
### 🍪 Task 5 - Cookie Tampering
🥅 Goal:
- Teach how to manipulate online session with cookie tampering

🔑 Key Takeway:
- Analyze requests to a web server and see if you can manipulate cookies or any headers within the HTTP request
- If you are able to decode cookie has with open source tools, you may be able to encode your own hash and send your own Session to authenticate as an Admin

## 🧠 Lessons Learned
- Ensuring that authentication mechanisms are secure are vital part of designing a highly secure web application.
- User Enumeration, Brute Force, exploiting Logic Flaws, and Cookie Tampering are ways to exploit vulnerabilities in authentication mechanisms.

🔗 Room Link:
[https://tryhackme.com/room/authenticationbypass](https://tryhackme.com/room/authenticationbypass)
