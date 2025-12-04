# Ethical Hacking Tools 🛡️💻

Welcome to our curated list of Ethical Hacking tools! Whether you're a beginner or an experienced pentester, these tools will aid you in various stages of your security assessments.

> "Tools are the subtlest of traps. We become reliant upon them and in their absence, we are vulnerable, weak, defenseless."

## Reconnaissance 🔍

### CLI // GUI

- [theHarvester](https://github.com/laramies/theHarvester) - Email and subdomain reconnaissance tool.
- [Wappalyzer](https://github.com/gokulapap/wappalyzer-cli) - Identify technologies used on websites.
- [recon-ng](https://github.com/lanmaster53/recon-ng) - Full-featured Web Reconnaissance framework.
- [dig](https://www.geeksforgeeks.org/dig-command-in-linux-with-examples/) - DNS information gathering tool.
- [traceroute](https://www.geeksforgeeks.org/traceroute-command-in-linux-with-examples/) - Discover the route taken by packets across an IP network.
- [sublist3r](https://github.com/aboul3la/Sublist3r) - Fast subdomains enumeration tool.
- [subfinder](https://github.com/projectdiscovery/subfinder) - Subdomain discovery tool.
- [urx](https://github.com/hahwul/urx) - URL discovery from archived webpages.

### Web-based 🌐

- [hunter.io](https://hunter.io) - Email hunter tool.
- [securitytrails.com](https://securitytrails.com) - Domain and IP intelligence tool.
- [crt.sh](https://crt.sh) - Certificate transparency search tool.
- [ctail](https://github.com/hdm/ctail.git) - CLI certificate transparency search tool.
- [shodan.io](https://shodan.io) - Search engine for Internet-connected devices.
- [predictasearch.com](https://www.predictasearch.com) - Discover exposed EPIs online.
- [epieos.com](https://epieos.com) - Discover exposed EPIs online.
- [grayhatwarfare.com](https://greyhatwarfare.com) - Search engine for finding open AWS S3 buckets.
- [dorkgenius.com](https://dorkgenius.com/) - Google dork generator.
- [generated.photos](https://generated.photos) - AI-generated stock photos.
- [overpass-turbo.eu](https://overpass-turbo.eu) - Query tool for OpenStreetMap data.
- [Wigle.net](https://wigle.net) - Wireless network mapping service.
- [grep.app](https://grep.app/) - Search code in repositories hosted on GitHub, GitLab, Bitbucket.

## Scan 📡

### Hosts/Ports Scanners

- [nmap](https://www.kali.org/tools/nmap/) - Network scanner and security audit tool.
- [nmap-scripts](https://nmap.org/book/man-nse.html) - Collection of NSE scripts.
- [rustscan](https://github.com/RustScan/RustScan) - Fast port scanner written in Rust.
- [naabu](https://github.com/projectdiscovery/naabu) - Fast port scanner.
- [massscan](https://github.com/robertdavidgraham/masscan) - Fast TCP port scanner.
- [hping3](https://www.kali.org/tools/hping3/) - TCP/IP packet assembler/analyzer.

### Vulnerability Scanners

- [nuclei](https://github.com/projectdiscovery/nuclei) - Fast and customizable vulnerability scanner.
- [OFFAT](https://github.com/OWASP/OFFAT) - Offensive Automation Framework And Tools.
- [nikto](https://www.kali.org/tools/nikto/) - Web server scanner.
- [trivy](https://github.com/aquasecurity/trivy) - Docker images scanner.

## Enumeration 📋

- [crackmapexec](https://github.com/byt3bl33d3r/CrackMapExec) - Swiss army knife for pentesting networks.
- [Impacket](https://github.com/fortra/impacket) - Collection of Python classes for working with network protocols.
- [NetExec](https://github.com/Pennyw0rth/NetExec-Wiki) - NetExec - Network Enumeration Tool for Windows/UNIX-based hosts.
- [smbclient](https://www.samba.org/samba/docs/current/man-html/smbclient.1.html) - Samba client tool.
- [ssh-enum (metasploit module)](https://www.infosecmatter.com/metasploit-module-library/?mm=auxiliary/scanner/ssh/ssh_enumusers) - SSH user enumeration module for Metasploit.
- [dirb](https://www.kali.org/tools/dirb/) - Web content scanner.
- [gobuster](https://github.com/OJ/gobuster) - Directory/file & DNS busting tool.
- [jwt-secrets](https://github.com/wallarm/jwt-secrets/blob/master/jwt.secrets.list) - List of default JWT secrets for cracking purposes.

## Exploitation 💥

### System Exploitation

- [metasploit](https://www.metasploit.com/) - Penetration testing framework.
    - meterpreter
    - msfvenom
- [CeWL](https://github.com/digininja/CeWL) - Custom Word List generator.
- [crunch](https://www.kali.org/tools/crunch/) - Password generator.
- [ncrack](https://nmap.org/ncrack/) - High-speed network authentication cracking tool.
- [CompanyPasswordGen](https://github.com/FenrirSec/CompanyPasswordGen) - Generate custom password lists.
- [hashcat](https://hashcat.net/hashcat/) - Password recovery tool.
- [johntheripper](https://github.com/openwall/john) - Password cracker.
- [onlinehashcrack.com](https://www.onlinehashcrack.com) - Online hash cracking service.
- [ntlm.pw](https://ntlm.pw) - NTLM hash database (every <= 9characters combinations).

### Web Exploitation

- [ffuf](https://github.com/ffuf/ffuf) - Fast web fuzzer.
- [burpsuite](https://portswigger.net/burp/communitydownload) - Java-based interception proxy and vulnerability scanner.
- [caido](https://caido.io/) - Interception proxy with a web (and also Electron) interface.
- [pwnloris](https://github.com/h0ussni/pwnloris) - Slowloris DoS attack tool.
- [sqlmap](https://sqlmap.org/) - Automatic SQL injection and database takeover tool.
- [p0wny webshell](https://github.com/flozz/p0wny-shell) - Simple web shell.
- [noSQLmap](https://github.com/codingo/NoSQLMap) - Automated NoSQL database enumeration and web application exploitation toolset.
- [httpx](https://github.com/projectdiscovery/httpx) - Fast and multi-purpose HTTP toolkit.

### Mobile Exploitation 📱

- [apktool](https://apktool.org/) - Reverse engineering Android APKs.
- [apkleaks](https://github.com/dwisiswant0/apkleaks) - Scanning APK file for endpoints and secrets.
- [hermes-dec (React Hermes Decompiler)](https://github.com/P1sec/hermes-dec) - Tool to decompile React Native apps.

### Decompilation
- https://pylingual.io/ (Python .pyc decompiler)

## Post-Exploitation 📝

### CLI // GUI

- [netcat](https://www.kali.org/tools/netcat/) - TCP/IP Swiss Army knife.
- [ncat](https://nmap.org/ncat/) - Netcat's reimplementation that supports encryption.
- [socat](https://www.kali.org/tools/socat/) - Multipurpose relay (SOcket CAT).
- [Peass-ng](https://github.com/peass-ng/PEASS-ng/tree/master) - Privilege Escalation Awesome Scripts Suite.
- [linenum.sh](https://github.com/rebootuser/LinEnum/tree/master) - Linux enumeration script.
- [termbin](https://termbin.com) - Command line pastebin.

### Web-Based

- [revshells.com](https://revshells.com) - Reverse shell cheat sheet generator.
- [CyberChef](https://gchq.github.io/CyberChef/) - Cyber operations data analysis tool.

## Reporting 📊

- [pwndoc](https://github.com/pwndoc/pwndoc) - Pentest report generator.

---

## General ℹ️

- [HackTricks](https://books.hacktricks.xyz) - The largest Red Team & Blue Team Cheat Sheet.
- [RockYou.txt](https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt) - Password dictionary.
- [prips](https://manpages.ubuntu.com/manpages/focal/man1/prips.1.html) - Generate IP address lists.
