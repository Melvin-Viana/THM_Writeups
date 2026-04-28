# 🔎 Content Discovery
- Platform: TryHackMe
- Difficulty: Easy
- Objective: Learn various ways of discovering hidden or private content on a webserver.
- Path: Jr. Penetration Tester
## 🧠 Overview
- Web applications haved hidden or non-public content that are sometimes left open to the public.
- Sensitive data needs to be hidden and in this room, ways to discover that data are explained in this room.

## 🔍 Methodology
  - First the room explains 3 ways of content discovery.
  - Then it explains different vulnerabilities exploited through "Manual" Content discovery.
  - Then using OSINT tools to discover content.
  - Ending with using scripts/tools to automate disovering content. 
--------
### 🚶‍♂️Task 1 - What is Content Discovery

🥅 Goal: 
- To inform what is content in a web application. 
- To educate how to discover content

💡 Key Takeway: 
- 3 Main ways of content discovery:
  1. Manual
  2. Automated
  3. OSINT (Open-Source Intelligence)
-------
### 🧭 Task 2 - Manual Discovery - Robots.txt
🥅 Goal:
- To inform what "robots.txt" in a web server does for a web app.

💡 Key Takeway: 
- Robots.txt is a simple text file that provides instructions to web crawlers about which pages or files they cannot access on a website.
- Shows endpoints that web server owner does not want public to access.
-------
### 🧭 Task 3 - Manual Discovery - Favicon
🥅 Goal:
- To educate about favicon's in web apps.

💡 Key Takeway: 
- Replace favicon because default favicon gives information as to what framework the web app may be using.
- OWASP has a database for favicons
- Find the md5sum of the icon
-------
### 🧭 Task 4 - Manual Discovery - Sitemap.xml
🥅 Goal:
- To educate about Sitemap.xml in web apps.

💡 Key Takeway: 
- Opposite of Robots.txt, where sitemap.xml lists every file the web app owner wants to share on web crawlers.
---------
### 🛜 Task 5 - Manual Discovery - HTTP Headers
🥅 Goal:
- To educate about HTTP Headers used when requests are made to web servers

💡 Key Lessons
- HTTP headers contain useful information about the webserver software and programming language used.
- Use the curl command to simulate a http request
---------
### 🛜 Task 6  - Manual Discovery - Framework Stack
🥅 Goal:
- To educate about web app frameworks

💡 Key Lessons
- Web app framework comments may be littered throughout the HTML code
- Frameworks may have information on vulnerabilities within their documentation
- Using developer tools you can discover Network requests made:
  - i.e. logging in is a POST request, you can simulate a POST request with:
    curl -X POST
---------
### 🕵️‍♂️ Task 7 - OSINT - Google Hacking/Dorking
🥅 Goal:
- To educate about discovering Open-Source intelligence on target through Google features.

💡 Key Lessons
- Google's advanced search engine features  allow for picking up certain search terms:
  - i.e. "Admin" URL endpoints
- https://en.widipedia.org/wiki/Google_hacking

### 🕵️‍♂️ Task 8 - OSINT - Wappalzyer
🥅 Goal:
- To educate about wappalyzer tool, discovers information on the web server and app framework(s).

---------
### 🕵️‍♂️ Task 9 - OSINT - Wayback Machine
🥅 Goal:
- To show how to go through archives of websites using Wayback Machine tool
---------
### 🕵️‍♂️ Task 10 - OSINT - Github
🥅 Goal:
- To explain what Git and Github is
---------
### 🕵️‍♂️ Task 11 - OSINT - S3 Buckets
🥅 Goal:
- To teach about Amazon AWS's storage service and its common bucket format - {name}.s3.amazonaws.com
---------
### 🤖 Task 12 - Automated Discovery
🥅 Goal:
- Using automation tools to discover features and flaws on a web app

💡 Key Lesson
- The are many different content discovery tools available; use wordlists to discover vulnerabilities
--------

## 🧠 Lessons Learned
- Three different ways to discover content on web applications:
  1. Manual
  2. OSINT
  3. Automated Discovery => Scripts
- Developer tools help in doing Manual content discovery
- Using default settings in frameworks cause vulnerabilities

🔗 Room Link:
[https://tryhackme.com/room/contentdiscovery](https://tryhackme.com/room/contentdiscovery)
