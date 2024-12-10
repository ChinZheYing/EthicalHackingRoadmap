# Ethical Hacking Roadmap

### Preface
Numbered points are to be read/watched in sequence, bullet/alphabet points can be read/watched in any sequence. This document focuses on the technical aspect of hacking (ignoring certifications/job requirements) as that is something I lack experience in.

Start off with the basics such as passive and active recon, exploitation, privilege escalation. Play with Metasploitable 2. Do CTFs. Tryhackme has a free path [Link](https://tryhackme.com/r/resources/blog/free_path).

Learn to program. Pick at least one compiled language (such as C, C++, C#, Rust, etc) and one interpreted language (such as Python, JS). Learn one native system language such as (Bash, Powershell) for each OS.

Now you can start specializing in fields such as web exploitation, exploit dev, malware dev, forensics etc. You shouldn't need much handholding at this point.
### 1) Basics
1. [TCM Ethical Hacking](https://youtu.be/3FNYvj2U0HM?si=XVhi1r5Ez66rmzVg) on YouTube (link might not be the latest version)
2. Privilege Escalation
	- [TCM Linux Privilege Escalation](https://youtu.be/ZTnwg3qCdVM?si=RlfTRS-nmMcIOEYo)
	- [TCM Windows Privilege Escalation](https://youtu.be/uTcrbNBcoxQ?si=K2EIGFbaZysaJCMw)

Practice your skills:
- Metasploitable
- Tryhackme
- PicoCTF
- Hack the box
### 2) Programming
Some people consider programming to be non-essential in hacking but imho it is ESSENTIAL. You can only break a system if you know how it works.
- C for exploit development, malware development and other low level stuff. Also good for programs that needs to be fast however this is less of a concern in 2024.
	1. C Programming A Modern Approach for basics
- Python for creating scripts for repetitive tasks, making hacking tools, attacking vulnerabilities. Python Flask is also used for web development. 
	1. Basics should've be taught in [TCM Ethical Hacking](https://youtu.be/3FNYvj2U0HM?si=XVhi1r5Ez66rmzVg)
	2. Black Hat Python hacking related Python stuff
	3. Learn threading
	4. Learn TKinter as it is the standard GUI library
	5. Learn Flask for web dev (optional but recommended)
	6. Make your own tools (only with standard Python libraries)
		- Netcat (Covered in Black Hat Python)
		- Wireshark clone. This will deepen your understanding of networking protocols down to the bits and bytes
		- NMAP clone (Advanced programmers can try to implement service version detection and os detection). Most of this is applying what you learned in Black Hat Python. Service detection requires you to learn about regex and probing.
		- Dirb clone (implement recursion, extensions)
		- Hydra clone (SSH and SFTP might be challenging without libraries like Paramiko. Using OpenSSH is OK)
		- Burp Suite clone (Yes, without libraries so no using Requests). This will deepen your understanding of how requests, headers and websites work.
- Web dev (HTML, JS, PHP, SQL, NoSQL) these are the most common languages that makes up a website. 
	1. Learn HTML and JS and make your own website. You can also host it on Firebase for free. Who knows when this might come in handy.
	2. Learn SQL and NoSQL
	3. Learn PHP
	4. Learn other frameworks such as NextJS, ReactJS. This shouldn't be too hard if you've done steps i-iii.
- Bash (TO BE COMPLETED)
- Powershell (TO BE COMPLETED)
### 3a) Web exploitation
1. Learn to build websites (which resource???)
2. Port swinger academy (Updated version of with labs The Web Application Hackers Handbook)
3. Tryhackme Web Application Pentesting (Optional if you don't want to pay)

Try practice your skills:
- OWASP Juice Shop
- DVWA (comes with Metasploitable)
### 3b) Exploit development (TO BE COMPLETED)
Buffer overflow used to be in OSCP but was removed due to it being rarely used in professional pentests; however, it is still a very fun topic and makes you less reliant on existing exploits that you don't understand
1. Pre requisite: C, Python
2. Liveoverflow's [Binary Exploitation playlist](https://www.youtube.com/playlist?list=PLhixgUqwRTjxglIswKp9mpkfPNfHkzyeN) on YouTube
3. [TCM Buffer Overflow](https://youtu.be/ncBblM920jw?si=ruz6eAMcSqUuMn8-)
4. Hacking the Art of Exploitation
5. Liveoverflow's [Sudo Vulnerability playlist](https://youtube.com/playlist?list=PLhixgUqwRTjy0gMuT4C3bmjeZjuNQyqdx&si=lkCAfE9Oaw-HljhP) on YouTube
### 3c) Malware development (TO BE COMPLETED)
Mostly focused on Windows malware development (such as Powershell, C# and win32 API). Linux malwares can be developed with programming languages learned in Part 2.
1. [Cosmodium Malware Dev playlist](https://youtube.com/playlist?list=PL_dk67mLCSFHa5jDNvEuXuoafMHmTjn32&si=BmpiiE-5T5-gjFwf) on YouTube

Projects to make:
- Keylogger (Included in Cosmodium playlist)
- Screenshots (Included in Cosmodium playlist)
- RAT (Included in Cosmodium playlist)
- C2 server with Python (Included in Cosmodium playlist)
- GUI C2 server with TKinter or Flask
- Ransomware
### 3d) Active Directory (TO BE COMPLETED)
Less likely to encounter if only playing around in CTF. Recommended for those looking to work in cyber field or taking certifications such as OSCP that contains AD.
1. [TCM AD Course](https://youtu.be/VXxH4n684HE?si=DCNlJgpLSmrvSNNY) Great as TCM guides you through building the AD environment before teaching exploitation. Need to have a decent computer.
2. Tryhackme AD contents (only for premium users tho...)
### 3e) OPSEC
Learn basic concepts (a lot of them are just basic logic that we neglect)
- Command and Control (C2)
- SSH Tunnelling
- Proxies
- VPN
- Tor, TailOS
- Changing MAC Address
