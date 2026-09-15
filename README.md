# networkwalks-b083-wk2-penetration-testing-report
## FOOTPRINTING & NETWORK SCANNING PHASES
W2-PM-FINAL | CYBERSECURITY |  NETWORKWALKS
* Pentester Name (Cybersecurity Professional): Iffrah Nauman
* Program/Batch: B083-Networkwalks
* Date: 16 september 2026
* Modules completed: W2-PM1 (Mutiple Kali Tools) W2-PM3 (Maltego) W2-PM5 (Zenmap scanning)
* Client/Target: Networkwalks (secured permission already) | My own local LAN network
* Permission secured from client: Yes
* Phases covered: Phase 1: Reconnaissance and Footprinting
                  Phase 2: Scanning and network discovery
                  Phase 3-5: In progress
  ## 1. Liability disclaimer
  I have performed these activities only on the systems & devices where I had secured written permission or the devices/systems that I own myself. All these materials are for education and research purpose only. Do not use anything from here to break the law. The instructor, the authors and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job and a permanent record. In most countries unauthorised access is a crime even when nothing is damaged.
  ## 2. Introduction
  This report covers footprinting the networkwalks.com domain using multiple Kali Linux tools (W2-PM1) , W2-PM3 (Maltego) and scanning my own local network with Zenmap (W2-PM5). One module covers the footprinting phase and the other covers the scanning phase, so together they show how an attacker moves from gathering public information to mapping live hosts on a network. It is the Week 2 part of my ongoing internship program at Networkwalks.
All commands were run in Kali Linux (footprinting) , maltego and on a Windows PC with Zenmap installed (scanning). Every step below includes the exact command used, the result I observed, a screenshot as evidence, and a short note on why the finding matters from an attacker's point of view.
## 3. Tools used
below are the list of tools used and their purpose
* Kali Linux & Windows : Operating system used for reconnaissance activity
* WHOIS: find domain registration details(owner , dates , names , server)
* whatweb: web technologies used (IP , server )
* nslookup: resolve domain name to its IP
* curl -l: tells HTTP response headers
* wafw00f: tells whether there is firewall protecting the site
* dnsrecon: all DNS records
* Maltego: tool used for OSINT and reconnaissance.( tells which information is connected which person , domain , company etc)
* Zenmap(Nmap GUI): scans the local subnet to find live hosts , IPs and MAC addresses
* Windows CMD: local IP and MAC address identification
## 4. Activities Performed
### 4.1 Footprinting and Reconnaissance
I performed reconnaissance/footprinting against networkwalks to find information about target. I used six kali tools to collect information. firstly , i used WHOIS which give us all publicaly available information about domain name , registrar , domain ID , domain server etc. The second tool i used was whatweb which gives information about web technologies used like IP address , server , email , HTTP server and WordPress 7.0.4 and WP download manager. after that i used nslookup which resolves the domain name to it's IP address. it resolved networkwalks.com into 192.232.216.135. the fourth tool i used was curl -l  which provides us with all information about HTTP response headers , wordpress , type:applicaton/json , path. the 5th tool i used was wafw00f it tells us whether a firewall is protecting a site or not. we get the result that the site is behind modsecurity. the last kali tool i used is dnsrecon it tells us about all dns records (TXT , NS ) related to mail records.
I also performed reconnaissance with maltego which is an OSINT tool it tells us which information is related to which person , compamy etc). I used the Transform → Utilities → To Email Address option to investigate email-related information. The transform used the information already available in the graph to identify related email information and display the relationships between the entities.
