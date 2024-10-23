There are many possible ways in which security could be compromised.n Those are possible ways an attacker could compromise systems. Those types of attacks are divided in *Technological Attacks* and *Social Engineering Attacks*.
### **Technological Attacks**

1. **IP Spoofing (Masquerading)**
	- **Description**: An attacker forges the source network address (usually IP) to impersonate a client or server. This type of of attack is possible because when using TCP the packet contains an header with the information of the IP address of the original server. But this packet is easily modifiable, allowing hackers to impersonate servers or other people. This type of attack is used mainly when the hackers has the control of the replies sent by the victim or is not interested in those replies.
    - **Countermeasures**: The main countermeasure is to do not trust addresses (either MAC or IP), but to use [[SOME SECURITY PRINCIPLES, C.I.A. TRIAD AND ABSTRACT SECURITIES PRINCIPLES|some sort of authentication]] either single or mutual.
2. **Packet Sniffing (Eavesdropping)**
    - **Description**: It's the unauthorized reading of network traffic by a malicious entity. 
    - **Countermeasures**: It can be avoided using encryption and applying the principle of [[SOME SECURITY PRINCIPLES, C.I.A. TRIAD AND ABSTRACT SECURITIES PRINCIPLES|integrity of data]]
1. **Connection Hijacking (Data Spoofing)**
    - **Description**: Similar to packet sniffing, the attacker takes control of an active communication session but this time to insert, delete, or manipulate data. It is also called *MITM* attack which stands for Man In The Middle Attack. This is an example that proves that you cannot trust the network and you have to take additional measures such, again, as [[ENCRYPTION|encryption]]. 
    - **Countermeasures**: Encryption, authentication, integrity checks.
4. **Denial-of-Service (DoS)**
    - **Description**: An attacker overloads a system to make it unavailable to users. This can be performed in various ways, usually trough ping requests or other forms of normal connections that cannot be distinguished from normal traffic.
    - **Countermeasures**: You can't!!!! Unfortunately there is not a single way or guideline on how you can prevent this. The best way is to distribute your system and keep multiple servers that can host your web-page or web-service.
5. **Distributed Denial-of-Service (DDoS)**
    
    - **Description**: Attackers use a botnet of compromised devices to multiply the effect of a DoS attack. This is quite intelligent because the attacker uses the botnet to perform the attack,but he directly disconnects before the attack takes place so he could be no more traceable. This bot-net usually work with a type of hierarchical structure where there are masters and zombies/daemons. Masters are simple nodes that are promoted to masters that can control various daemons. So the attacker connect to the bot-net trough the masters and then disconnect before the masters can forward the request to the controlled daemons. 
    - **Countermeasures**: No foolproof countermeasures, mitigation through robust architecture and monitoring.
6. **Shadow/Fake Server**
    - **Description**: This type of attack is deeply connected with IP spoofing. In this attack the hacker tries to impersonate a server to gain data on the user. Usually this type of attack can be performed if the attacker knows he is faster than the original server, or either controls the local DNS server or attacked the original server with a DDos attack so it can't be reached.
    - **Countermeasures**: Server authentication with the principle of [[SOME SECURITY PRINCIPLES, C.I.A. TRIAD AND ABSTRACT SECURITIES PRINCIPLES|mutual authentication]].
7. **Trojan**
    - **Description**: A malicious program disguised as legitimate software, typically containing harmful payloads.
    - **Countermeasures**: User education, anti-virus, secure software practices.
8. **Virus and Worms**
    - **Virus**: Damages the system and replicates through user action.
    - **Worm**: Self-replicating malware that spreads without human intervention.
    - **Countermeasures**: Anti-virus software, system patches, secure configurations.
9. **Ransomware**
    - **Description**: Malware that encrypts data and demands payment for decryption. This type of attack is very common, especially in large public or private organizations. The software usually include a detailed guide on how you can proceed with the payment of the ransom(often trough bitcoin). But this type of payment, more often than not, does not unlock the full data either because of the hacker grief(they want to extort as much money as possible) or because even them do not possesses anymore the keys due to law enforcement intervention and seize of the ransomware server where the keys are stored.
    - **Countermeasures**: Regular backups, keeping security patches up to date, anti-ransomware tools.

## Social engineering attacks
All this type of technological attacks could be very complicated and advanced and the complexity of the countermeasure could also follow the same path. But everything pale in confrontation to the humans faulty behaviors on a system. In the end humans will be always the week chain ring of a system. Those are the principal type of attacks that could be performed on humans.
### Phishing

Phishing is the use mail or similar tools to attract a user to a fake (shadow) server to. The goal for the attacker is to acquire their personal data or persuade them to install a plugin or extension (which actually is a virus or a Trojan).

There are two main variants of phishing:

- **Spear phishing**: includes several personal data to disguise the fake message as a good one (e.g. e-mail address, name of Dept/Office, phone number, etc.)
- **Whaling**: in this case the attacker utilizes spear phishing methods to go after a large, high-profile target, such as a CEO or CIO.

### Fake mail

Faking an email or a SMS is easy, the difficult part is using the right tone to trick the victim. In emails a way to circumvent this problem could be using a previous real email and changing parts of it (for example an attachment). SMS are easier to fake since they are usually shorter.


## Examples of Attacks
#### 1. T.J. Maxx Attack (2007)

The T.J. Maxx cyberattack is one of the most infamous early examples of a major data breach. The attack occurred over 18 months, up to January 2007, and resulted in the theft of 45 million credit and debit card numbers. The attack was carried out by a group of ten individuals from various countries, including the United States, Ukraine, China, Belgium, and Estonia. One of the key enablers of the attack was T.J. Maxx’s use of the Wired Equivalent Privacy (WEP) protocol, which had known vulnerabilities. WEP was significantly less secure than its replacement, WPA (Wi-Fi Protected Access), yet T.J. Maxx had not upgraded its security systems to align with state-of-the-art protections.

The attackers exploited WEP’s weaknesses to gain unauthorized access to the retailer's network and subsequently extracted massive amounts of sensitive customer data. The aftermath of the breach was extensive, including a class-action lawsuit from 300 banks and a total legal cost of $10 million for the company​​.

**Lessons Learned**: The T.J. Maxx breach highlights the importance of updating security protocols as technology evolves. In this case, failure to replace WEP with WPA resulted in severe consequences. Organizations must stay ahead of technological vulnerabilities by adopting the latest security measures, such as more secure encryption protocols. Regular audits and updates to security systems are critical in protecting customer data from exploitation.

#### 2. Phishing via Transformers 3 (2010)

In April 2010, a phishing attack targeted personnel at Andersen Air Force Base on Guam during an Operational Readiness Exercise (ORE). The phishing message falsely claimed that the movie _Transformers 3_ would be filmed on Guam and sought to recruit 20 airmen as extras. To apply, participants were asked to disclose sensitive personal information. The phishing attempt was exposed when an airman shared the opportunity on a fan blog for the _Transformers_ series, leading journalists to inquire about the film shoot. This raised awareness of the phishing attack.

Phishing emails are crafted to appear as legitimate communications, tricking recipients into providing personal details or credentials. In this case, the attackers capitalized on the excitement surrounding a popular film to lure military personnel into revealing sensitive information​.

**Lessons Learned**: The _Transformers 3_ phishing attempt underscores the need for cybersecurity awareness, especially within military and government environments. Social engineering tactics that play on emotional responses, such as excitement or urgency, can lead individuals to fall victim to scams. Regular training on how to recognize and avoid phishing attacks is essential, as is the enforcement of strict protocols for handling sensitive information.

#### 3. Stuxnet (2010)

Stuxnet was a sophisticated worm that first came to light in 2010 and marked a turning point in the realm of cyber warfare. Unlike most malware, which primarily targets personal or corporate data, Stuxnet was designed to sabotage industrial control systems, specifically Iran's nuclear enrichment facilities. The worm spread through Windows systems and was highly targeted, aiming to damage SCADA (Supervisory Control and Data Acquisition) systems used in industrial processes.

Stuxnet was particularly dangerous because it exploited four zero-day vulnerabilities in Windows systems. It likely gained entry to the network through a USB drive used by a maintenance worker. Once inside, it spread through network shares and attacked the control systems responsible for the centrifuges used in uranium enrichment, causing physical damage to the equipment without being detected for a considerable time.

The worm's distribution across several countries, particularly Iran, where over 50% of the infections occurred, sparked widespread concerns about the implications of cyber-attacks on national infrastructure​​.

**Lessons Learned**: Stuxnet highlighted the vulnerability of critical infrastructure to cyber-attacks. It revealed that even highly isolated systems with air gaps can be compromised if adequate cybersecurity measures (such as regular patching and disabling unnecessary services) are not in place. This case serves as a reminder to maintain strong defenses even for systems that are not directly connected to the internet, and to be vigilant about the use of removable media.

#### 4. Fancy Bear (APT28)

Fancy Bear, also known as APT28, is a Russian hacking group believed to be connected to the GRU, Russia's military intelligence agency. The group has been involved in numerous cyber espionage campaigns targeting political organizations, media outlets, and military entities across Europe and the United States. Notable targets include the German Bundestag, French TV station TV5Monde, the White House, NATO, and the U.S. Democratic National Committee (DNC) during the 2016 U.S. presidential election.

Fancy Bear is known for using spear-phishing attacks, malware, and other hacking techniques to steal sensitive information and manipulate public opinion. One of its most notable operations involved leaking thousands of emails from the DNC, a move that significantly influenced the political landscape during the 2016 election​​.

**Lessons Learned**: Fancy Bear’s activities underscore the growing threat of state-sponsored cyber espionage and the potential for cyber-attacks to influence political processes. It emphasizes the importance of advanced threat detection, the use of multifactor authentication to protect sensitive communications, and robust incident response plans for handling targeted attacks on high-profile organizations.

#### 5. Mirai (2016)

Mirai was a botnet that emerged in 2016, leveraging a massive network of compromised Internet of Things (IoT) devices, such as cameras, routers, and baby monitors, to launch devastating Distributed Denial-of-Service (DDoS) attacks. The botnet was responsible for some of the largest DDoS attacks ever recorded, including an attack on the cybersecurity blog _Krebs on Security_, which reached a bandwidth of 620 Gbps, and another on the DNS provider Dyn, which disrupted major websites like Twitter, Netflix, and Reddit.

Mirai spread by scanning the internet for devices that still had default factory usernames and passwords. Once it compromised these devices, it transformed them into bots that could flood targets with overwhelming amounts of traffic. Mirai's creators released the source code to the public, leading to the rise of similar botnets​.

**Lessons Learned**: The Mirai attack exposed the vulnerabilities of IoT devices, many of which lack basic security protections, such as password hardening or the ability to receive firmware updates. This incident underscored the need for manufacturers to build security into IoT devices from the start and for consumers to change default credentials and apply patches as soon as they become available.