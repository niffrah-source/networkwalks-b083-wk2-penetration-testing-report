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
  ## Liability disclaimer
  I have performed these activities only on the systems & devices where I had secured written permission or the devices/systems that I own myself. All these materials are for education and research purpose only. Do not use anything from here to break the law. The instructor, the authors and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job and a permanent record. In most countries unauthorised access is a crime even when nothing is damaged.
  ## Introduction
  This report covers footprinting the networkwalks.com domain using multiple Kali Linux tools (W2-PM1) , W2-PM3 (Maltego) and scanning my own local network with Zenmap (W2-PM5). One module covers the footprinting phase and the other covers the scanning phase, so together they show how an attacker moves from gathering public information to mapping live hosts on a network. It is the Week 2 part of my ongoing internship program at Networkwalks.
All commands were run in Kali Linux (footprinting) , maltego and on a Windows PC with Zenmap installed (scanning). Every step below includes the exact command used, the result I observed, a screenshot as evidence, and a short note on why the finding matters from an attacker's point of view.
## Tools used
below are the list of tools used and their purpose
* Kali Linux & Windows : Operating system used for reconnaissance activity
* WHOIS: find domain registration details(owner , dates , names , server)
* whatweb: web technologies used (IP , server )
* nslookup: resolve domain name to its IP
* curl -l: tells HTTP response headers
* wafw00f: tells whether there is firewall protecting the site
* dnsrecon: all DNS records
* Maltego: 
