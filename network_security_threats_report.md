# \#***Network security threats***

These are malicious acts, vulnerabilities, or confidentiality, integrity, or availability of an organisation's digital network and data. These threats manifest as unauthorized access attempts, data interception, service disruptions, or infrastructure compromises. Some of the common network security threats are DoS attack, Man-In-The-Middle attack(MITM), and spoofing.

#### ***#Dos attacks***

Denial of service originates from single system, it makes computer network system and network unavailable to its users by flooding it over whelming amounts of traffic or requests, consuming its resources like CPU or memory.

It works by

* **overwhelming target:** it means generating large and massive amount of requests(HTTP requests, ping packets) to overwhelm the target's by flooding all requests to exploit bandwidth or CPU.
* **resource exhaustion:** exploiting vulnerabilities in network protocols(like TCP) to leave half open connections hanging, quickly depleting connection requests.
* **service interruption**: simulating normal user behaviour like repeatedly reloading a complex webpage or executing heavy database researches to specifically cripple the application level.

###### ***# working of DoS in detail***



A DoS attack works in a step-by-step manner:



**2.1 Target Identification**

The attacker first selects a target such as a website, server, or network system.



**2.2 Sending Malicious Traffic**

The attacker sends a large number of requests or packets to the target system.



**2.3 Resource Exhaustion**

The system’s resources such as CPU, memory, or bandwidth get exhausted due to excessive requests.



**2.4 Service Disruption**

As a result, the system becomes slow or completely unavailable for legitimate users.



\---



**3. Types of DoS Attacks**



**3.1 Volume-Based Attacks**

These attacks aim to consume the bandwidth of the target.



**Working:**

A huge amount of traffic is sent to the system, which overloads the network and blocks legitimate traffic.



Examples:



\* UDP Flood

\* ICMP (Ping) Flood



\---



**3.2 Protocol-Based Attacks**

These attacks target weaknesses in network protocols.



**Working:**

The attacker sends incomplete connection requests. The server keeps waiting for completion and allocates resources, which eventually get exhausted.



Example:



\* SYN Flood Attack



\---



**3.3 Application Layer Attacks**

These attacks target the application layer (Layer 7).



**Working:**

The attacker sends multiple valid-looking requests to the server. These requests consume processing power and make the application slow or crash.



Examples:



\* HTTP GET/POST Flood

\* Slowloris Attack







**4. Impacts of DoS Attacks**



**4.1 Service Downtime**

The system becomes unavailable to users.



**4.2 Financial Loss**

Companies may lose revenue due to service interruption.



**4.3 Resource Exhaustion**

CPU, memory, and bandwidth usage increase significantly.



**4.4 Reputation Damage**

Users lose trust in the service or organization.



**4.5 Security Risks**

DoS attacks may be used as a distraction to perform other attacks.



\---



**5. Mitigation Techniques**



**5.1 Firewalls and Filtering**

Firewalls can block suspicious traffic and unauthorized access.



**5.2 Rate Limiting**

Limits the number of requests from a single user or IP.



**5.3 Load Balancing**

Distributes traffic across multiple servers to reduce load.



**5.4 Content Delivery Network (CDN)**

Helps absorb large traffic and improves availability.



**5.5 Intrusion Detection and Prevention Systems (IDS/IPS)**

Detects and blocks malicious traffic patterns.



**5.6 SYN Cookies**

Protects against SYN flood attacks by validating connections.



**5.7 Web Application Firewall (WAF)**

Filters application-level traffic and blocks malicious requests.



**5.8 Auto Scaling**

Increases resources automatically during high traffic.



**5.9 IP Blocking and Geo-Blocking**

Blocks suspicious IP addresses or regions.



\---



**6. Conclusion**

&#x20;  Denial of Service attacks are a major threat to system availability. They can cause serious financial and operational damage. These attacks work by overwhelming system resources or exploiting vulnerabilities. However, by using proper security measures such as firewalls, CDNs, WAFs, and intrusion detection systems, organizations can effectively prevent and mitigate DoS attacks. A layered security approach is essential to ensure continuous service availability.



\---



**7. Key Points**



\* DoS attacks target availability

\* Three types: Volume, Protocol, Application

\* SYN Flood is a common example

\* DDoS is a distributed and more powerful version

\* Prevention requires multiple security layers



**## DoS Attack Diagram**



![DoS Attack](https://raw.githubusercontent.com/rekhanjalikoya-dot/network_security_threats_report/main/dos.png)



### \#***Man-In-The-Middle Attack(MITM)***

***Man-in-the-Middle (MITM) Attack: Working, Impact and Mitigation***



***1. Introduction***

&#x20;  A Man-in-the-Middle (MITM) attack is a type of cyberattack in which an attacker secretly intercepts and possibly alters the communication between two parties without their knowledge. The attacker positions themselves between the sender and receiver, making both parties believe they are communicating directly with each other. MITM attacks mainly affect confidentiality and integrity in the CIA triad***.***



***---***



***2. Working of MITM Attack***



A MITM attack works in a step-by-step manner:



**2.1 Interception**

The attacker intercepts the communication between two users, such as a client and a server.



**2.2 Establishing Connection**

The attacker creates separate connections with both parties and acts as a relay between them.



**2.3 Data Monitoring or Manipulation**

The attacker can read, modify, or inject malicious data into the communication.



**2.4 Forwarding Data**

The modified or original data is forwarded to the intended receiver without raising suspicion.



\---



***3. Types of MITM Attacks***



***3.1 ARP Spoofing***

***Working:***

The attacker sends fake ARP (Address Resolution Protocol) messages to associate their MAC address with the IP address of a legitimate device. This allows the attacker to intercept traffic in a local network.



***---***



***3.2 DNS Spoofing***

***Working:***

The attacker redirects a user to a fake website by altering DNS responses. The user unknowingly enters sensitive data on the malicious site.



***---***



***3.3 Session Hijacking***

***Working:***

The attacker steals session cookies to gain unauthorized access to a user’s session without needing login credentials.



***---***



***3.4 SSL Stripping***

***Working:***

The attacker downgrades a secure HTTPS connection to HTTP, allowing them to view and modify unencrypted data.



***---***



***3.5 Wi-Fi Eavesdropping***

***Working:***

The attacker sets up a fake or unsecured Wi-Fi network to capture user traffic.



***---***



***4. Difference Between MITM and DoS***



***MITM (Man-in-the-Middle):***



***\**** Focuses on intercepting communication

\* Aims to steal or modify data

\* Targets confidentiality and integrity



***DoS (Denial of Service):***



***\**** Focuses on making services unavailable

\* Overloads system resources

\* Targets availability



***---***



***5. Impacts of MITM Attacks***



***5.1 Data Theft***

Sensitive information such as passwords, credit card details, and personal data can be stolen.



***5.2 Data Manipulation***

Attackers can modify messages, leading to incorrect or malicious information.



***5.3 Identity Theft***

Stolen credentials can be used to impersonate users.



***5.4 Financial Loss***

Unauthorized transactions may occur.



***5.5 Loss of Privacy***

User communication is exposed to attackers.



***---***



***6. Mitigation Techniques***



***6.1 Use of HTTPS***

Always use secure HTTPS connections to encrypt communication.



***6.2 SSL/TLS Certificates***

Ensure websites use valid and trusted digital certificates.



***6.3 Virtual Private Network (VPN)***

Encrypts network traffic and prevents interception.



***6.4 Secure Wi-Fi Usage***

Avoid using public or unsecured Wi-Fi networks.



***6.5 Two-Factor Authentication (2FA)***

Adds an extra layer of security even if credentials are stolen.



***6.6 ARP Inspection***

Detects and prevents ARP spoofing attacks in networks.



***6.7 DNS Security (DNSSEC)***

Prevents DNS spoofing by validating DNS responses.



***6.8 Firewall and IDS/IPS***

Monitors and blocks suspicious activities.



***---***



***7. Conclusion***

&#x20;  Man-in-the-Middle attacks are a serious security threat that compromise the confidentiality and integrity of communication. Attackers secretly intercept and manipulate data between two parties. These attacks can lead to data theft, financial loss, and identity misuse. However, by using strong encryption methods, secure communication protocols, and proper security tools, MITM attacks can be effectively prevented.



***---***



***8. Key Points***



***\**** MITM attacks intercept communication between two parties

\* Targets confidentiality and integrity

\* Common types: ARP spoofing, DNS spoofing, SSL stripping

\* Can lead to data theft and identity fraud

\* Prevention includes HTTPS, VPN, and strong authentication



**## MITM Attack Diagram**



![MITM Attack](https://raw.githubusercontent.com/rekhanjalikoya-dot/network_security_threats_report/main/mitm.png)




### ***#Spoofing Attack***



Spoofing Attack: Working, Impact and Mitigation



**1. Introduction**

&#x20;  Spoofing is a type of cyberattack in which an attacker impersonates a legitimate user, device, or system to gain unauthorized access, steal data, or bypass security mechanisms. In spoofing attacks, the attacker falsifies identity-related information such as IP address, email address, or website identity. Spoofing mainly affects confidentiality, integrity, and authentication in the CIA triad.



\---



**2. Working of Spoofing Attack**



A spoofing attack works in a step-by-step manner:



**2.1 Target Identification**

The attacker selects a target such as a user, network, or organization.



**2.2 Identity Forgery**

The attacker creates a fake identity by modifying technical information such as IP address, email headers, or DNS records.



**2.3 Gaining Trust**

The victim believes the attacker is a legitimate source and interacts with them.



**2.4 Exploitation**

The attacker uses this trust to steal sensitive data, spread malware, or gain unauthorized access.



\---



**3. Types of Spoofing Attacks**



**3.1 IP Spoofing**

**Working:**

The attacker modifies the source IP address in packets to make them appear as if they are coming from a trusted system. This is often used in DoS/DDoS attacks.



\---



**3.2 Email Spoofing**

**Working:**

The attacker sends emails with a forged sender address, making it look like the email is from a trusted source such as a bank or company.



\---



**3.3 DNS Spoofing**

**Working:**

The attacker alters DNS records to redirect users to malicious websites instead of legitimate ones.



\---



**3.4 ARP Spoofing**

**Working:**

The attacker sends fake ARP messages to link their MAC address with a legitimate IP address, allowing them to intercept network traffic.



\---



**3.5 Website Spoofing**

**Working:**

The attacker creates a fake website that looks identical to a real one to trick users into entering sensitive information.



\---



**4. Difference Between Spoofing and MITM**



**Spoofing:**



\* Focuses on impersonating identity

\* Used to gain trust of the victim

\* May lead to further attacks



**MITM (Man-in-the-Middle):**



\* Focuses on intercepting communication

\* Attacker sits between two parties

\* Can use spoofing as a technique



\---



**5. Impacts of Spoofing Attacks**



**5.1 Data Theft**

Sensitive information such as login credentials and financial data can be stolen.



**5.2 Unauthorized Access**

Attackers may gain access to systems or accounts.



**5.3 Malware Distribution**

Spoofed emails or websites can deliver malicious software.



**5.4 Financial Loss**

Victims may lose money due to fraud or phishing attacks.



**5.5 Reputation Damage**

Organizations may lose trust if their identity is spoofed.



\---



**6. Mitigation Techniques**



**6.1 Authentication Mechanisms**

Use strong authentication methods to verify identities.



**6.2 Email Security Protocols**

Implement SPF (Sender Policy Framework), DKIM (DomainKeys Identified Mail), and DMARC to prevent email spoofing.



**6.3 Encryption**

Use secure communication protocols such as HTTPS and SSL/TLS.



**6.4 Network Security Measures**

Enable ARP inspection and use secure network configurations.



**6.5 DNS Security (DNSSEC)**

Ensures authenticity of DNS responses.



**6.6 User Awareness**

Educate users to identify suspicious emails and websites.



**6.7 Firewalls and IDS/IPS**

Detect and block suspicious activities.



\---



**7. Conclusion**

&#x20;  Spoofing attacks are a major security threat that involve impersonating trusted entities to deceive users and systems. These attacks can lead to data theft, unauthorized access, and financial loss. However, by implementing strong authentication, encryption, and security protocols, spoofing attacks can be effectively prevented.



\---



**8. Key Points**



\* Spoofing involves impersonation of identity

\* Common types: IP, Email, DNS, ARP, Website spoofing

\* Used to gain trust and exploit victims

\* Can lead to data theft and financial fraud

\* Prevention includes authentication, encryption, and awareness


 
**## Spoofing Attack Diagram** 



![Spoofing Attack](https://raw.githubusercontent.com/rekhanjalikoya-dot/network_security_threats_report/main/spoofing.png)










