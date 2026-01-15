
# Tools

## Nmap (+nping)
> get it from apt, package name `nmap`

Network scanner and port scanner tool.

Also comes with nping tool, for sending custom packets. 

Scripts can be found here: https://nmap.org/nsedoc/scripts/

### Common useful scripts
* `vulners` detects potential vulnerabilites
* `ipv6-ra-flood` can flood something with with fake routers to bog it down
* `jdwp-exec` can try to detect if a Java debug port could potentially be exploited

## Sqlmap
> https://github.com/sqlmapproject/sqlmap

Automatic SQL injection and database takeover tool. Can scan for injections and exploit them.

## Wireshark
> get it from apt, package name `wireshark`

Packet sniffing and analyzing, mostly useful for local network hacking. Run it with `sudo wireshark`.

## Metasploit Framework

> get it from the docs: https://docs.metasploit.com/docs/using-metasploit/getting-started/nightly-installers.html

A versatile toolbox for hackers loaded with tons of exploits and useful stuff. De facto exploiting tool.

## Aircrack-ng
> install via apt, package id `aircrack-ng`, or build from source

A tool for packet sniffing and cracking wifi passwords.

## Nikto
> install via apt, pakcage `nikto`

An all in one tool for scanning web servers and sites for potential vulnerabilites or security issues.

## Scapy
> install via apt, package `python3-scapy`

An extremely versatile python based packet manipulation tool.

## EvilLimiter
> install from https://github.com/bitbrute/EvilLimiter

An ARP spoofing tool for limiting or blocking devices on the local network.

## macchanger
> install via apt

Literally does what it says on the tin.

## Ghidra
> install from https://github.com/NationalSecurityAgency/ghidra

The NSA's open source reverse engineering framework.
*Yes, that NSA.*

## CloakQuest3r
> https://github.com/spyboy-productions/CloakQuest3r

"Uncover the true IP address of websites safeguarded by Cloudflare & Others."

## hping3
> install via apt

An easy to use simple packet crafting, smashing, and flood tool.

## mat2
> install via apt

A tool for cleaning metadata off files.

## pixload
> https://github.com/sighook/pixload

A tool for embedding metasploit payloads and malware inside image files, good for exploiting file uploads.

## wafw00f
> install via apt

This is a tool for detecting if a website is behind a WAF, and if so identifying what it is.

## exiftool
> install via apt

A tool for editing and modifying metadata of files.

## gobuster
> install via apt

Tool designed to use wordlists to find hidden webpages.

## hydra
> install via apt

A password cracking/guessing tool. Very useful and versatile, can work on a variety of things.

## searchsploit
> https://gitlab.com/exploit-database/exploitdb

A database of useful exploits, that can be installed locally.

## 403-bypass
> https://github.com/thediablo1337/403-bypass

Tool for getting around "403 forbidden" HTTP errors.

## nomore403
> https://github.com/devploit/nomore403

Tool for getting around "403 forbidden" HTTP errors, written in go. you will have to know how to compile/build it from source.

## dnstwist
> https://github.com/elceef/dnstwist | https://dnstwist.it

Tool for finding phishing domains based on typos.

## mitmproxy
> https://docs.mitmproxy.org/stable/overview/installation

A very versatile MITM proxy. An *essential* tool for intercepting requests and manipulating data of websites. Comes with an easy to use `mitmweb` interface.

A free tool instead of something like Burp Suite, and mitm could honestly be considered better in some regards.

**Todo: install guide**

## arp-scan
> install via apt

Does what it says on the tin. Can also do a bit more.

## SecLists
> https://github.com/danielmiessler/SecLists

A github repo full of lists of common usernames and stuff, great if you need a wordlist.

## hashcat
> install via apt

A tool for cracking password hashes. You will need a powerful GPU/CPU for using this.

## mimikatz
> https://github.com/gentilkiwi/mimikatz

A tool for extracting windows passwords and PINs from memory. 

## curl
> already installed in every distro

Tool for transferring data from a server using URLs. Basically command line web requests.

## netcat (aka nc)
> sudo apt install nc

Netcat is a tool for arbitrary TCP and UDP listening and connections. Very userful for data transfer and *reverse shells*.

## whatweb
> https://github.com/urbanadventurer/WhatWeb

A tool written in Ruby.

"WhatWeb identifies websites. Its goal is to answer the question, "What is that Website?". WhatWeb recognises web technologies including content management systems (CMS), blogging platforms, statistic/analytics packages, JavaScript libraries, web servers, and embedded devices. WhatWeb has over 1800 plugins, each to recognise something different. WhatWeb also identifies version numbers, email addresses, account IDs, web framework modules, SQL errors, and more." 

## ncat
> sudo apt install ncat

Not to be confused with `netcat`. "Ncat is a feature-packed networking utility which reads and writes data across networks from the command line."

## binwalk
> sudo apt install binwalk

Tool for searching bin files and binary images for embeddded files and executable code.


# Misc Vulnerabilites
**NOTICE: THIS SECTION EXCLUDES ANYTHING ON EXPLOITDB, BECUASE YOU CAN JUST GO LOOK THAT UP EZ**

## openSSH 9.7 RCE
* https://github.com/Karmakstylez/CVE-2024-6387
* https://github.com/d0rb/CVE-2024-6387

## openSSH 9.2 traffic forwarding
* https://github.com/TX-One/CVE-2023-38408

## openSSH 8.3 RCE
Note: requires devices to be on same local network, so is not as usable except maybe in an attack chain
*  https://github.com/Neko-chanQwQ/CVE-2020-15778-Exploit
## HikVision Camera Exploiting
* https://github.com/tamim1089/HikvisionExploiter

# Useful Websites
## exploit-db
> https://www.exploit-db.com/

A large database of known exploits and tooling for them. Very useful.

## CVEFeed
> https://cvefeed.io/

A site that watches for new CVEs, and trawls github for potential exploits for them.

## pentestmonkey
> https://pentestmonkey.net/category/cheat-sheet

A site with a few useful cheat sheets and such.

## Hacksplaining (Lessons)  
> https://www.hacksplaining.com/lessons

A fun little site that can show you how some basic attacks work, for free.

## VirusTotal
> https://www.virustotal.com/gui/home/upload

Everyone knows what VirusTotal is.

## WhereGoes
> https://wheregoes.com/

A link and redirect checker. Useful for looking at phishing links to see where they go.

## Hackviser (Tactics)
> https://hackviser.com/tactics/pentesting

A normally paid site that has some pretty neat free guides.

## Shodan
> https://www.shodan.io/

A site that scans the internet for open devices. Shows how insecure everything really is.

## censys
> https://search.censys.io/

Kind of like Shodan, but more for websites.

## cyberchef
> https://cyberchef.org/

A useful website for manipulating strings, especially obfuscated ones.

## vim cheat sheet
> https://vim.rtorr.com/

read the title

## GTFOBins
> https://gtfobins.github.io/ 

“GTFOBins is a curated list of Unix binaries that can be used to bypass local security restrictions in misconfigured systems.”

## URLHaus Abuse.ch
> https://urlhaus.abuse.ch/browse/

A place where active malware URLs are logged. Good for target practice.

## Hacktricks
> https://book.hacktricks.wiki/en/index.html 

A very nice pentesting and hacking resource with *tons* of info.

## crt.sh
> https://crt.sh

A website that can check DNS to find hidden subdomains.

## OWASP Cheat Sheets
> https://cheatsheetseries.owasp.org/index.html

A bunch of useful cheatsheets.

## OWASP Web Application Pentest Guide
> https://owasp.org/www-project-web-security-testing-guide/

## OWASP Web Security Testing Guide
> https://owasp.org/www-project-web-security-testing-guide/stable/

What it says on the tin.

## Reverse Shell File Transfer Cheatsheet
> https://www.hackingarticles.in/file-transfer-cheatsheet-windows-and-linux/

## Powershell Obfuscator
> https://powershellobfuscator.com/

## MITRE ATT&CK
> https://attack.mitre.org/

A list of how all the threat groups actually get away with stuff and their methods. Stuff like persistence and yknow.

## Persistence Cheatsheet
> https://hackmag.com/security/persistence-cheatsheet

For reverse shell antics.
## Offensive-Payloads
> https://github.com/InfoSecWarrior/Offensive-Payloads/tree/main

A bunch of useful payloads for different injection testing.

## Extension: Wappalyzer
> https://addons.mozilla.org/en-US/firefox/addon/wappalyzer/

Firefox extensions for analyzing what websites run. May want to disable data collection. Is a semi-SaaS product, so be careful.

## Dork_Search
> https://dorksearch.com/

A web-based google dorking service.

## ghostwriter Documentation
> https://ghostwriter.kde.org/documentation/

Read the title. Also a useful markdown cheatsheet.  

## DDG Advanced Search Docs
> https://duckduckgo.com/duckduckgo-help-pages/results/syntax

How to use advanced search features, which can be used for dorking.

# Privacy/Security Stuff

## Mullvad VPN
> https://mullvad.net/en

The best VPN. Been raided by the feds multiple times, they don't keep any logs. Unlike other VPN providers, they don't care what you do and allow you to do cybersec work.

**You will need to pay in BTC or ideally Monero XMR.**

***YOU SHOULD ALWAYS HAVE A VPN WHEN HACKING. RATHER SAFE THAN SORRY.***

## Tor Browser
> https://www.torproject.org/

The Tor broswer. How to access the dark web in addition to clearweb.

Keep in mind accessing the dark web is perfectly legal as long as you don't do anything illegal like sell drugs.
## torctl
> https://github.com/BlackArch/torctl
> https://github.com/a3oYzmN4fGhm7rA4ob/linuxmint-torctl-installer

A tool to route all your network traffic through tor.

## VeraCrypt
> https://veracrypt.io/en/Downloads.html

VeraCrypt is a free open source disk encryption software. It can create virtual encrypted disks within a file, or create encrypted partitons easily with a GUI. It also supports double hidden volume plausible deniability.

## Kleopatra
> https://apps.kde.org/kleopatra/

"Kleopatra is an open-source certificate manager and graphical front-end for cryptographic services, primarily designed to handle OpenPGP and S/MIME (X.509) certificates."

Basically, easy to use GUI PGP encryption tool. Very useful.

## Bisq
> https://bisq.network/

Decentralized p2p bitcoin exchange. No kyc. 
"Bisq is an open-source desktop application that allows you to buy and sell bitcoin in exchange for national currencies, or alternative cryptocurrencies."
# Random tools | sites
## dl-librescore
> https://github.com/LibreScore/dl-librescore

A tool for ripping sheet music from MuseScore.


## Easy Linux Tips | Security in Mint & Ubuntu
> https://easylinuxtipsproject.blogspot.com/p/security.html

A useful guide for explaining to new linux users why you don't need antivirus or slop.

## repak
> https://github.com/trumank/repak/releases/tag/v0.2.2

Useful tool for unpacking unreal engine files.

## Copyparty
> https://github.com/9001/copyparty/

"turn almost any device into a file server with resumable uploads/downloads using any web browser"  
  
A powerful FOSS file server, in a single python file. For a detailed breakdown, go to https://www.youtube.com/watch?v=15_-hgsX2V0.

## Konversation
> https://konversation.kde.org/download.html

KDE IRC client. Availbile on flathub.

# Additional resources for ppl who are learining, about privacy and cybersec

## YouTube

### Videos

[Wi-Fi Hacking Basics: Networking 101 For Ethical Hackers](https://www.youtube.com/watch?v=vxvAp9drxNg)

[Network Hacking Basics: Ports, HTTPS and Certificates](https://youtu.be/2Swg_oPNXq8)

[linux vs bill gates](https://youtu.be/KwnBZZ7_FGg)

[“I Have Nothing to Hide” – The Dangerous Myth About Privacy](https://youtu.be/Hcqh0ZSza50)

[I2P: A Comfy Guide (Connecting and Creating an I2P Website)](https://youtu.be/yOaSkXue5gE)

### Channels

[DeadOverflow (web pentesting and stuff)](https://www.youtube.com/@deadoverflow)

## Written Guides
