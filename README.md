WPScan is a WordPress security scanning tool used to identify vulnerabilities, plugins, themes, and users in WordPress websites.

⚠️ Warning: WPScan should only be used on authorized websites. Unauthorized scanning may be illegal.   

📌 Tool Information
```bash
Tool Name: WPScan

Version Used: 3.8.28

Platform: Linux (Parrot OS / Kali Linux)

Language: Ruby

Official Website: https://wpscan.com
```

🔧 Installation (As shown in photos)   
```bash
sudo gem install wpscan
```

🔍 Check WPScan Version
```bash
wpscan --version
```

Output:

WPScan Version 3.8.28

🌐 Basic WordPress Scan    
```bash
wpscan --url https://zinmatt.com/
```
What this does:

WordPress detection

Server & IP information

WordPress version check

Database update check

🚫 403 Forbidden Error (WAF Issue)    
```bash
wpscan --url https://excellencecoaching.in/
```

Error:

Scan Aborted: The target is responding with a 403, this might be due to a WAF.

✅ Solution: Use Random User-Agent    
```bash
wpscan --url https://excellencecoaching.in/ --random-user-agent
```
✔ It reduces the chances of being blocked by a Web Application Firewall (WAF).

🔎 Advanced Enumeration Scan   
```bash
wpscan --url https://zinmatt.com/ --enumerate u t vt vp --random-user-agent
```
Enumeration Flags Explained:    
```bash
Flag	Meaning
u	Enumerate users
t	Enumerate themes
vt	Vulnerable themes
vp	Vulnerable plugins
```
✔ Detailed vulnerability    
✔ Website IP address   
✔ Scan start time  
✔ Target confirmation

🛡️ Common Use Cases

WordPress security auditing

Bug bounty reconnaissance (authorized scope only)

Learning WordPress penetration testing

Defensive security testing

❗ Legal & Ethical Notice

⚠️ IMPORTANT:

Scan only your own website or a website for which you have written permission.

Unauthorized scanning may be considered a cyber crime.

Use this tool strictly for educational purposes only.

📚 References

WPScan Official: https://wpscan.com

Automattic (Sponsor): https://automattic.com

👨‍💻 Author

Created for learning & educational purposes
Tool demonstrated on Parrot OS
