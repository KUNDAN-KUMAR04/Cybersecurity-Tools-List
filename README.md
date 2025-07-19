# Cybersecurity-Tools-List: A Curated List of Cybersecurity & Penetration Testing Tools

A comprehensive and categorized index of essential tools for ethical hacking, cybersecurity, vulnerability assessment, and penetration testing. This repository aims to provide a quick reference for security enthusiasts, students, and professionals.

## Table of Contents
- [Disclaimer](#disclaimer)
- [How to Contribute](#how-to-contribute)
- [Categories](#categories)
    - [Network Scanning & Discovery](#network-scanning--discovery)
    - [Vulnerability Scanners](#vulnerability-scanners)
    - [Web Application Hacking](#web-application-hacking)
    - [Wireless Hacking](#wireless-hacking)
    - [Password Cracking](#password-cracking)
    - [Forensics & Reverse Engineering](#forensics--reverse-engineering)
    - [Operating Systems](#operating-systems)
    - [Exploitation Frameworks](#exploitation-frameworks)
    - [Social Engineering](#social-engineering)
    - [Cloud Security](#cloud-security)
    - [Container Security](#container-security)
    - [Threat Intelligence](#threat-intelligence)
    - [OSINT (Open Source Intelligence)](#osint-open-source-intelligence)
    - [Other Utilities](#other-utilities)
- [License](#license)

## Disclaimer

**IMPORTANT:** This repository lists tools that can be used for both legitimate cybersecurity purposes (e.g., penetration testing, vulnerability assessment) and potentially malicious activities. **Users are solely responsible for ensuring they have the legal authority and explicit permission to use these tools on any network or system.** Unauthorized access to computer systems is illegal and punishable by law. This repository is for educational and ethical purposes only.

## How to Contribute

We welcome contributions! If you know of a great tool that's not listed, or if you find an error, please:
1.  **Fork** this repository.
2.  Create a new **branch** (`git checkout -b feature/AddNewTool`).
3.  Add your tool to the appropriate category.
4.  Commit your changes (`git commit -m 'Add new tool: [Tool Name]'`).
5.  Push to your branch (`git push origin feature/AddNewTool`).
6.  Open a **Pull Request** explaining your changes.

## Categories

---

### Network Scanning & Discovery
* **[Angry IP Scanner (ipscan)](https://angryip.org/)**
    * *Description:* A fast and friendly network scanner. It scans IP addresses and ports and has many other features.
    * *Features:* Multi-threaded, highly configurable, extensible with plugins, can export results in various formats.
    * *Operating Systems:* Cross-platform (Java-based: Windows, macOS, Linux).
    * *License:* GPLv2
* **[Masscan](https://github.com/robertdavidgraham/masscan)**
    * *Description:* An Internet-scale port scanner. It can scan the entire Internet in under 5 minutes, transmitting 10 million packets per second.
    * *Features:* Asynchronous TCP port scanner, fast scanning.
    * *Operating Systems:* Linux, macOS, Windows.
    * *License:* MIT License
* **[Nmap](https://nmap.org/)**
    * *Description:* A free and open-source utility for network discovery and security auditing. Used for host discovery, port scanning, OS detection, and service version detection.
    * *Features:* Host discovery, port scanning, service/version detection, OS detection, scriptable interaction (Nmap Scripting Engine - NSE).
    * *Operating Systems:* Cross-platform (Linux, Windows, macOS).
    * *License:* GPLv2
* **[Wireshark](https://www.wireshark.org/)**
    * *Description:* A free and open-source network protocol analyzer. Captures and interactively browses traffic running on a computer network.
    * *Features:* Deep inspection of hundreds of protocols, live capture, offline analysis, rich VoIP analysis.
    * *Operating Systems:* Cross-platform.
    * *License:* GPLv2
* **[Zmap](https://zmap.io/)**
    * *Description:* An open-source network scanner that enables researchers to easily perform large-scale studies of the Internet. It can scan the entire IPv4 address space in under 45 minutes on a gigabit Ethernet connection.
    * *Features:* High-speed network scanning, supports various protocols (SYN, ICMP, UDP, etc.), flexible output.
    * *Operating Systems:* Linux, macOS.
    * *License:* GPLv2

### Vulnerability Scanners
* **[Nessus](https://www.tenable.com/products/nessus)**
    * *Description:* A proprietary vulnerability scanner developed by Tenable, Inc. Widely used for identifying vulnerabilities, misconfigurations, and compliance issues.
    * *Features:* Comprehensive vulnerability scanning, configuration auditing, patch management analysis.
    * *Operating Systems:* Cross-platform.
    * *License:* Commercial
* **[Nuclei](https://github.com/projectdiscovery/nuclei)**
    * *Description:* An open-source, template-based vulnerability scanner by ProjectDiscovery. It uses simple YAML-based templates to send requests, allowing for fast and extensive scanning for various vulnerabilities across targets.
    * *Features:* Template-based, fast and configurable, supports various protocols (HTTP, DNS, TCP, etc.), active community for templates.
    * *Operating Systems:* Cross-platform.
    * *License:* MIT License
* **[OpenVAS](http://www.openvas.org/) (Greenbone Vulnerability Management - GVM)**
    * *Description:* A full-featured vulnerability scanner and manager. The underlying technology is Greenbone Vulnerability Management (GVM), an open-source framework for network and application vulnerability scanning.
    * *Features:* Unauthenticated and authenticated testing, various high-level and low-level internet and industrial protocols.
    * *Operating Systems:* Linux (often deployed via Docker or dedicated packages).
    * *License:* GNU GPL
* **[OWASP ZAP (Zed Attack Proxy)](https://www.zaproxy.org/)**
    * *Description:* A free and open-source web application security scanner. It's one of the most popular DAST (Dynamic Application Security Testing) tools for finding vulnerabilities in web applications.
    * *Features:* Proxy, automated scanner, fuzzer, spider, active and passive scans, extensibility via marketplace.
    * *Operating Systems:* Cross-platform (Java-based).
    * *License:* Apache License 2.0

### Web Application Hacking
* **[Burp Suite](https://portswigger.net/burp)**
    * *Description:* An integrated platform for performing security testing of web applications. (Community Edition is free, Professional is paid).
    * *Features:* HTTP proxy, scanner, intruder, repeater, sequencer, decoder, comparer.
    * *Operating Systems:* Cross-platform (Java-based).
    * *License:* Community (Free), Professional (Commercial)
* **[DirBuster](https://github.com/OWASP/DirBuster)**
    * *Description:* A multi-threaded Java application designed to brute force directories and file names on web servers. It helps discover hidden files and directories.
    * *Features:* Multi-threaded, supports proxy, wordlist generation, configurable scan depth.
    * *Operating Systems:* Cross-platform (Java-based).
    * *License:* LGPL
* **[Nikto](https://cirt.net/Nikto2)**
    * *Description:* An open-source web server scanner that performs comprehensive tests against web servers for known vulnerabilities.
    * *Features:* Scans for over 6700 potentially dangerous files/CGIs, outdated server versions, and version-specific problems.
    * *Operating Systems:* Linux, Windows, macOS.
    * *License:* GPL
* **[SQLMap](http://sqlmap.org/)**
    * *Description:* An open-source penetration testing tool that automates the process of detecting and exploiting SQL injection flaws and taking over database servers.
    * *Features:* Extensive database support, various SQL injection techniques, database fingerprinting, data fetching, file access, command execution.
    * *Operating Systems:* Cross-platform (Python).
    * *License:* GPLv2
* **[Wfuzz](https://github.com/xmendez/wfuzz)**
    * *Description:* A tool designed for brute-forcing Web applications. It can be used for finding resources not linked (directories, servlets, scripts, etc.), brute forcing GET and POST parameters, checking for various kinds of injections.
    * *Features:* Highly configurable, supports various encoders, multiple output formats, proxy support.
    * *Operating Systems:* Cross-platform (Python).
    * *License:* GPLv2

### Wireless Hacking
* **[Aircrack-ng](https://www.aircrack-ng.org/)**
    * *Description:* A complete suite of tools to assess WiFi network security. Focuses on various aspects of WiFi security, including monitoring, attacking, testing, and cracking.
    * *Features:* WEP/WPA/WPA2-PSK cracking, packet injection, deauthentication.
    * *Operating Systems:* Linux, macOS, Windows (limited support).
    * *License:* GPLv2
* **[Kismet](https://www.kismetwireless.net/)**
    * *Description:* A wireless network detector, sniffer, and intrusion detection system. It identifies wireless networks by passively collecting packets and detecting non-beaconing networks.
    * *Features:* Passive scanning, network discovery, packet sniffing, client identification, WIDS (Wireless Intrusion Detection System).
    * *Operating Systems:* Linux, macOS, BSD.
    * *License:* GPLv2

### Password Cracking
* **[Hashcat](https://hashcat.net/hashcat/)**
    * *Description:* The world's fastest and most advanced password recovery utility. Supports a wide range of hashing algorithms and attack modes, leveraging GPU acceleration.
    * *Features:* Brute-force, dictionary, hybrid, mask, rule-based attacks. GPU accelerated.
    * *Operating Systems:* Linux, macOS, Windows.
    * *License:* MIT License
* **[John the Ripper](https://www.openwall.com/john/)**
    * *Description:* A popular open-source password cracker. Used to detect weak Unix passwords, but supports many other hash types.
    * *Features:* Dictionary attack, brute-force attack, custom rules.
    * *Operating Systems:* Cross-platform.
    * *License:* GPLv2

### Forensics & Reverse Engineering
* **[Autopsy (The Sleuth Kit)](https://www.autopsy.com/)**
    * *Description:* An open-source digital forensics platform used for analyzing hard drives and smartphones. It's the graphical user interface for The Sleuth Kit (TSK), providing a comprehensive set of investigative tools.
    * *Features:* Timeline analysis, keyword search, web artifact analysis, email analysis, data carving, extensibility via modules.
    * *Operating Systems:* Windows, Linux, macOS.
    * *License:* GPLv3
* **[Ghidra](https://ghidra-sre.org/)**
    * *Description:* A software reverse engineering (SRE) framework developed by the NSA. Helps analyze compiled code (e.g., executables, libraries).
    * *Features:* Disassembler, decompiler, graphical interface.
    * *Operating Systems:* Cross-platform (Java-based).
    * *License:* Apache License 2.0
* **[IDA Pro (Interactive Disassembler Professional)](https://hex-rays.com/ida-pro/)**
    * *Description:* A proprietary, multi-processor disassembler and debugger that translates machine-executable code into assembly language. Widely considered the industry standard for reverse engineering.
    * *Features:* Supports numerous processors, interactive analysis, FLIRT signatures, debugger integration, scripting.
    * *Operating Systems:* Windows, Linux, macOS.
    * *License:* Commercial (IDA Freeware available with limitations)
* **[Volatility Framework](https://www.volatilityfoundation.org/)**
    * *Description:* An open-source memory forensics framework for extracting digital artifacts from volatile memory (RAM) dumps.
    * *Features:* Process listing, network connection analysis, registry analysis, rootkit detection.
    * *Operating Systems:* Cross-platform (runs on Python).
    * *License:* GPLv2

### Operating Systems
* **[Kali Linux](https://www.kali.org/)**
    * *Description:* A Debian-based Linux distribution designed for digital forensics and penetration testing. Comes pre-installed with hundreds of tools.
    * *Features:* Wide array of pre-installed security tools, customizable, active community.
    * *Operating Systems:* Linux.
    * *License:* GPLv2 (and others for individual tools)
* **[Parrot Security OS](https://www.parrotsec.org/)**
    * *Description:* A Debian-based Linux distribution similar to Kali, focused on security, privacy, and development.
    * *Features:* Security tools, privacy-focused apps, lightweight.
    * *Operating Systems:* Linux.
    * *License:* GPL (and others)

### Exploitation Frameworks
* **[Covenant](https://github.com/cobbr/Covenant)**
    * *Description:* An open-source .NET command and control (C2) framework that aims to be a collaborative and modern alternative to other C2s.
    * *Features:* Multi-user support, various listeners (HTTP, SMB), C# and PowerShell implants, tasking and reporting.
    * *Operating Systems:* Cross-platform (.NET Core).
    * *License:* MIT License
* **[Metasploit Framework](https://www.metasploit.com/)**
    * *Description:* A powerful open-source penetration testing framework. Provides a platform for developing, testing, and executing exploits.
    * *Features:* Exploit modules, payloads, encoders, post-exploitation modules.
    * *Operating Systems:* Cross-platform.
    * *License:* BSD-style

### Social Engineering
* **[SET (Social-Engineer Toolkit)](https://github.com/trustedsec/social-engineer-toolkit)**
    * *Description:* An open-source Python-driven tool designed for social engineering attacks, such as phishing, credential harvesting, and spear phishing.
    * *Features:* Phishing attacks, tabnabbing, web jacking, infectious media generator.
    * *Operating Systems:* Linux.
    * *License:* GPL

### Cloud Security
* **[CloudGoat](https://github.com/RhinoSecurityLabs/CloudGoat)**
    * *Description:* A deliberately vulnerable AWS environment designed to teach and practice cloud penetration testing. It's a "capture the flag" style exercise.
    * *Features:* Reproducible vulnerable AWS scenarios, learning environment.
    * *Operating Systems:* Cross-platform (Python, requires AWS account).
    * *License:* MIT License
* **[Pacu](https://github.com/RhinoSecurityLabs/Pacu)**
    * *Description:* An open-source AWS exploitation framework designed for offensive security operations in Amazon Web Services environments.
    * *Features:* Various modules for reconnaissance, privilege escalation, data exfiltration, and resource manipulation within AWS.
    * *Operating Systems:* Cross-platform (Python).
    * *License:* MIT License
* **[Prowler](https://github.com/prowler-cloud/prowler)**
    * *Description:* An open-source tool for AWS security assessment, auditing, hardening, and incident response. It follows AWS security best practices.
    * *Features:* Checks over 200 AWS security best practices, compliance frameworks.
    * *Operating Systems:* Linux, macOS.
    * *License:* Apache License 2.0
* **[ScoutSuite](https://github.com/nccgroup/ScoutSuite)**
    * *Description:* An open-source multi-cloud security auditing tool that enables security posture assessment of cloud environments.
    * *Features:* Audits AWS, Azure, GCP, Alibaba Cloud, Kubernetes.
    * *Operating Systems:* Cross-platform (Python).
    * *License:* GPLv3

### Container Security
* **[Clair](https://github.com/quay/clair)**
    * *Description:* An open-source tool for static analysis of vulnerabilities in application containers. It provides an API that analyzes images and indexes common vulnerabilities.
    * *Features:* Static container image analysis, integrates with registries, vulnerability database.
    * *Operating Systems:* Linux (containerized deployment).
    * *License:* Apache License 2.0
* **[Docker Bench for Security](https://github.com/docker/docker-bench-security)**
    * *Description:* A script that checks for common best practices in deploying Docker containers in production. Based on the CIS Docker Benchmark.
    * *Features:* Automated security checks, easy to run.
    * *Operating Systems:* Linux (Docker required).
    * *License:* Apache License 2.0
* **[Trivy](https://aquasecurity.github.io/trivy/)**
    * *Description:* A comprehensive and easy-to-use vulnerability scanner for containers, filesystems, and Git repositories.
    * *Features:* Scans OS packages, application dependencies, IaC configurations.
    * *Operating Systems:* Cross-platform.
    * *License:* Apache License 2.0

### Threat Intelligence
* **[MISP (Malware Information Sharing Platform)](https://www.misp-project.org/)**
    * *Description:* An open-source platform for sharing, storing, and correlating Indicators of Compromise (IOCs) of targeted attacks, cyber security incidents, and malware.
    * *Features:* Event management, attribute management, sharing, correlation.
    * *Operating Systems:* Linux.
    * *License:* AGPLv3

### OSINT (Open Source Intelligence)
* **[Maltego](https://www.maltego.com/)**
    * *Description:* A graphical link analysis tool for gathering and connecting information for investigative tasks.
    * *Features:* Data mining, information gathering, relationship visualization.
    * *Operating Systems:* Cross-platform.
    * *License:* Commercial (Community Edition available)
* **[Shodan](https://www.shodan.io/)**
    * *Description:* A search engine for Internet-connected devices. Finds devices like servers, routers, webcams, and industrial control systems.
    * *Features:* Device search, network mapping, vulnerability identification.
    * *Operating Systems:* Web-based (API available).
    * *License:* Commercial (Free tier available)
* **[theHarvester](https://github.com/laramies/theHarvester)**
    * *Description:* A simple, yet effective tool for gathering open-source intelligence. It collects emails, subdomains, hosts, employee names, open ports, and banners from various public sources.
    * *Features:* Integrates with search engines (Google, Bing, Yahoo), PGP servers, LinkedIn, DNS dumpsters, etc.
    * *Operating Systems:* Cross-platform (Python).
    * *License:* GPLv3
* **[Twint](https://github.com/twintproject/twint)**
    * *Description:* An advanced Twitter scraping tool written in Python that allows for scraping Twitter tweets without Twitter's API. *Note: As of late 2023/early 2024, Twint's functionality is heavily impacted by Twitter API changes and its maintenance status is uncertain.*
    * *Features:* Scraping tweets from user timelines, followers, following, hashtags, keywords, location, and more.
    * *Operating Systems:* Cross-platform (Python).
    * *License:* GPLv3

### Other Utilities
* **[hping3](http://www.hping.org/)**
    * *Description:* A command-line oriented TCP/IP packet assembler/analyzer. Useful for firewall testing, port scanning, network testing using different protocols, and more.
    * *Features:* Custom packet creation, firewall testing, DoS testing.
    * *Operating Systems:* Linux.
    * *License:* GPL
* **[Netcat (nc)](https://www.gnu.org/software/netcat/)**
    * *Description:* A simple Unix utility that reads and writes data across network connections using TCP or UDP. Known as the "TCP/IP Swiss Army knife."
    * *Features:* Port scanning, banner grabbing, backdoor, file transfer.
    * *Operating Systems:* Cross-platform.
    * *License:* GPL
* **[Vagrant](https://www.vagrantup.com/)**
    * *Description:* A tool for building and managing virtual machine environments. Useful for setting up isolated labs for testing cybersecurity tools and malware analysis.
    * *Features:* Portable development environments, supports VirtualBox, VMware, Docker, automatic provisioning.
    * *Operating Systems:* Cross-platform.
    * *License:* MIT License

## License

This project is licensed under the [MIT License](LICENSE).
