---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# Baseline
---
- Security vs convenience
	- <u>More security can lead to less convenience</u>
	- By making things more difficult for users it may lead to less security
	- Balance needed
- Types of security ^5689a1
	- Information Security
		- Act of protecting <u>data and information</u> from unauthorized access, unlawful modification, disruption, disclosure, corruption, and destruction
		- Data that system is holding <u>NOT</u> the system itself
	- Information System Security
		- Securing the <u>systems</u> that hold and process critical data
		- System holding data but <u>NOT</u> the actual data

# Cybersecurity Models
---
- CIA ^51b6d8
	- Confidentiality ^9c173d
		- Ensuring info is not being disclosed to unauthorized people
		- [[Disk Encryption#^501400|Encryption]] can keep data confidential
	- Integrity ^1f11b5
		- Confirm data has not been modified in any way by unauthorized people without permission
		- #Hashing or Journaling showing an audit trail
	- Availability ^3803a7
		- Data easily and readily accessible to authorized users
		- Stored, accessible, and protected at all times
		- Creating redundancy, error handling, and having software free from bugs
		- #Uptime
- AAA ^45fffd
	- Authentication
		- <u>Proof of identity</u> and systems confirms
		- Methods:
			- Something you know
				- User/Pass
			- Something you are
				- Finger/Eye
			- Something you have
				- Token/card
			- Something you do
				- Way you speak or sign
			- Somewhere you
				- Geolocation/Subnet
	- Authorization
		- Occurs when <u>user is given access to certain data</u> or area
		- Indicates the level or <u>amount</u> of access you have
	- Accounting
		- Tracking data, computer usage, and network resources are maintained
		- <u>Logging</u>
		- <u>Non-Repudiation</u>
			- Proof someone did something
-  Objectives
	- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]

# Security threats
---
- [[Malware]]
	- Malicious software
		- [[Viruses]]
		- [[Worms]]
		- [[Trojans]]
		- [[Spyware]]
			- [[Spyware#Adware|Adware]]
		- [[Rootkits]]
		- [[Ransomware]]
- Unauthorized access
	- Occurs when access to computer resources and data <u>happens without consent</u> of the owner
	- Breaking through <u>authorization</u>
- System Failure
	- Computer crashes or an application fails
		- [[Symptoms of Infection]]
	- BSOD
		- Occurs when there is a crash on the PC. Indicates a serious issue in #Windows ^e2abc0
		- [[Symptoms of Infection]]
	- Affecting <u>availability</u>
- #SocialEngineering
	- <u>Manipulating user to reveal</u> confidential information or perform action detrimental to user or company
	- Phishing
- Objectives
	- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
	- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]

# Mitigating Threats
---
- Physical controls
	- Alarms, locks, cameras, ID cards, guards
- Technical Controls ^c5223f
	- Smart cards, ACL, [[IDS]]/IPS, network authentication
- Administrative Controls ^50e62d
	- AKA "Managerial Controls"
	- Policy, procedures, awareness, training, disaster recovery
		- User training one of the most cost effective methods
	- Sub categories
		- Procedural
			- Company policy
		- Legal/Regulatory
			- Adhering to standards and laws
			- PCI, HIPPA,etc???
- Objectives
	- [[Objectives#5.1 - Compare and contrast various types of controls|5.1 - Compare and contrast various types of controls]]

# Hackers
---
- White Hats
	- Not malicious
	- <u>Work for company</u>
	- "Ethical hackers or Pen Testers"
- Black Hats
	- Bad actors
	- Try to get in without permission or authorization
	- Bad guys
- Grey Hats
	- White/Black
	- <u>No affiliation</u>
	- Risk breaking law
	- <u>May not have malicious intent</u>
	- Hacking for the sake of hacking not to cause damage
	- Still breaking the law in general but may responsibly disclose
- Blue Hats
	- Attempting to hack into company at their request
	- <u>Freelancer or contractor</u>
	- Bug bounty
- Elite Hats
	- <u>The "best"</u>
	- Find 0 days
	- Create own tools
	- White. Black, Grey hats
	- '1/10,000 considered'
- #Script Kiddies
	- <u>Low level of skill</u>
	- Use tools without understanding
- Objectives
	- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]

# Threat Actors
---
- #Script Kiddies
	- <u>No/Little skill or ability</u>
	- Blindly use tool
- Hacktivists
	- <u>Driven by cause</u> terrorism, social justice, etc
- Organized crime
	- Group of <u>hackers well-funded</u> and sophisticated
- Advanced Persistent Threats ^f3f779
	- <u>Nation state</u>, covert, #OSINT
	- Gain more #Intelligence and info
	- Often maintain a <u>low profile</u>
	- Can take place over longer periods off time
- Objectives
	- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]

# Threat #Intelligence

## Assessing #Intelligence
---
- Weighing value of #Intelligence
	- Timeliness
		- Is it up to date?
		- Less valuable over time
	- Relevancy
		- Information is relevant to your use case
		- Does it affect your organization?
		- Ex: #OSX hacks in a #Windows environment are likely not relevant
	- Accuracy
		- Produces <u>productive results</u>
		- <u>Valid and true</u> info
		- Checking AI and ML alerts
	- Confidence
		- Producing <u>qualified statements</u>
		- <u>MISP</u> rating
			- Codifies use of admiralty scale for grading data and estimative language
			- <u>Source reliability</u>
				- Letter grade A - F
				- Reliable, Usually reliable, Fairly reliable, Not usually reliable, Unreliable, Cannot be judged
			- <u>Information content</u>
				- Number 1 - 6
				- Confirmed, Probably true, Possibly True, Doubtfully True, Improbable, Can't be judged
- Objectives
	- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]

## Sources
---
- Proprietary
	- <u>Paid commercial</u> services
	- May not have own data and just aggregate others
- Closed
	- Data <u>derived from their own research</u> from analysis and reports
	- FireEye - Proprietary with closed data
- [[#^36c7e3|Open]] #OSINT
	- Data <u>openly available</u> without subscription
	- Reputation lists and [[Malware]] signature databases
	- US-CERT
		- Computer emergency readiness team
		- Regular reports, analysis, bulletins
		- Bidirectional threat feed ^15c875
			- Automatic Indicator Service
	- NCSC
		- UK style US-CERT
	- AT&T Security (OTX)
		- Previously AlienVault Open Threat Exchange
	- MISP
		- [[Malware]] Information Sharing Project
	- VirusTotal
		- Upload file and checks across 40+ [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]]
		- Public repo
	- Spamhaus
		- [[Spam]] #Email
	- SANS ISC
		- ISC Suspicious domain
- Threat feeds
	- <u>Explicit knowledge</u>
		- Knowledge you can write down, see, or touch ^c4a1c4
	- <u>Implicit knowledge</u>
		- Experienced practitioners analysis ^b8800d
		- "Sense" what is wrong
		- Ability to have attitude and instinct
		- Can't write down. Purely Experience
- #OSINT
	- Open Source #Intelligence
	- Obtain info about person/company via public records websites, social media ^36c7e3
	- Enumeration scans
- Objectives
	- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]

# Threat Hunting
---
- Cyber security technique designed to <u>detect presence of threats not discovered by normal security monitoring</u> ^2a9491
- Is a <u>proactive method vs reactive</u> such as in Incident Response
- Potentially less disrupting than pen test
	- Analyze data within systems you already have
- Process
	- Hypothesis
		- Based from threat model and based on <u>potential events with higher likelihood and impact</u>
		- Who would harm us?
		- How would they harm us?
	- Profiling Threat Actors
		- Create scenarios how intrusion might happen and what motive is TTP
			- Tactics, Techniques, Procedures ^a6b869
		- Who wants to cause harm?
		- What systems?
	- Hunting
		- Using tools for regular security and IR
			- Logs, file, registry changes
			- A #SIEM
		- Assume regular security systems have failed
		- Examples
			- Network traffic analysis
				- List of suspicious hosts
			- Check executables on hosts
				- Confirm validity of processes
			- Check other hosts
				- Compare similarities
			- Identify how the [[Malware]] came about
- Can consume a lot of resources but can yield some benefits
	- Improve detection capabilities
	- Integrate new info into #Intelligence
		- Corelating external info with internal logs
		- Actionable #Intelligence
	- Reduce attack surface
	- Block attack vectors
	- Identify critical assets
		- Improve monitoring around those systems
- Objectives
	- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]

# Attack Frameworks

## Lockheed Martin Kill Chain
---
- About
	- First made under contract
	- Release to public eventually
	- <u>Linear</u> outside from perimeter to inside path
	- Somewhat older
- Steps
	- #Reconnaissance
		- Attacker determines <u>methods to use to attack</u>
			- [[Malware Infections#Attack Vector|Attack Vector]]
		- Attackers try to have a low profile
			- [[Endpoint Analysis#Advanced Threat Protection (ATP)|Advanced Threat Protection (ATP)]]
		- Use #OSINT and passive tools
		- Go from passive to active scanning/actions
		- Identifying where/how to attack target
	- Weaponization
		- Attackers couple #Payload with #Exploit  code
		- Creating tool but <u>NOT running</u>
	- Delivery
		- Attacker finds vector for #Payload
		- [[Malware Infections#Threat vector|Threat vector]]
	- Exploitation
		- The moment code is executed and running
		- "Phase 1"
	- Installation
		- During #Exploit it will install additional code to maintain remote access and achieve persistence
		- "Phase 2"
	- Command and Control #C2 ^5ba0e4
		- Where weaponized code talks to an outside server to use additional functions
		- Able to remotely use host at this point
		- Establish 2 way communication
	- Actions on objectives
		- Whatever the goal is
			- Data extraction, Damage, etc
- Map out security plan based on steps
	- Detect, deny, disrupt, degrade, deceive, destroy

## MITRE ATT&CK Framework
---
- Adversary tactics, technique, and common knowledge
- <u>Attack navigator</u>
	- attack.mitre.org
	- Can click different types and colors to get TTP
	- Each one will give you more info
	- Map of possible methodology for attack and defense
- Knowledge based maintained by MITRE organization
- More iterative or thinking across multiple lines
	- Matrices
	- Many categories of attacks
- <u>Focus</u> on [[Disk Encryption#^501400|Encryption]] phase
- pre-ATT&CK
	- Focus on #Reconnaissance
	- Aligns with #Reconnaissance and weaponization in Lockheed kill chain [[#Attack Frameworks]]
	- Detect before it is a problem

## Diamond Model of Intrusion analysis
---
- Focus on <u>intrusion event</u>
- Categories
	- Victim
	- Capability
	- Adversary
	- #Infrastructure
- For each incident you want to map the event out
- Flow
	- Victim notices/discovers [[Malware]]
	- Ability to see you've been hacked
	- As you do IR you may see a #C2 server being called
		- This will point to a #Infrastructure
	- Firewall logs can point to an IP being accessed by several hosts
		- Additional information on #Infrastructure and victim discovery
	- IP details add info on Adversary
- Once all is identified <u>define a tuple</u>
	- A finite ordered list of elements ^d9cef6
	- Create an array with 4 categories and other metadata
	- "E = {something}"
	- Helps with an automated info like a #SIEM
- Models can be used individually or combined

```ad-info
title: Diamond Model
collapse:close
![[Diamond-Model.png]]
```

```ad-info
title: Diamond Model Tuple
collapse:close
![[Diamond-E=.png]]
```

```ad-info
title: Combined Models
collapse:close
![[CombinedModels.png]]
```

# Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]
- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]
- [[Objectives#4.2 - Summarize the importance of policies, processes, and procedures for incident response|4.2 - Summarize the importance of policies, processes, and procedures for incident response]]
- [[Objectives#5.1 - Compare and contrast various types of controls|5.1 - Compare and contrast various types of controls]]