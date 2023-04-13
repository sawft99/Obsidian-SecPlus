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
		- Act of protecting <u>data and information</u> from unauthorized access, unlawful modification, disruption, disclosure, corruption, and destruction ^276bff
		- Data that system is holding <u>NOT</u> the system itself
	- Information System Security
		- Securing the <u>systems</u> that hold and process critical data ^71e062
		- System holding data but <u>NOT</u> the actual data

# Cybersecurity Models
---
- CIA ^51b6d8
	- Confidentiality
		- Ensuring info is not being disclosed to unauthorized people ^b8c85d
		- [[Disk Encryption#^501400|Encryption]] can keep data confidential
	- Integrity
		- Confirm data has not been modified in any way by unauthorized people without permission ^00e120
		- #Hashing or Journaling showing an [[#^45fffd|Audit]] trail
	- Availability
		- Data easily and readily accessible to authorized users ^59133d
		- Stored, accessible, and protected at all times
		- Creating redundancy, error handling, and having software free from bugs
		- #Uptime
- AAA ^45fffd
	- Authentication
		- When a persons identity is established with proof and confirmed by a system ^80ee75
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
		- Occurs when <u>user is given access to certain data</u> or area ^bca181
		- Indicates the level or <u>amount</u> of access you have
	- Accounting
		- Tracking data, computer usage, and network resources are maintained
		- <u>Non-Repudiation</u>
			- Proof someone did something ^4e6600
		- AKA
			- <u>Auditing</u>
			- <u>Monitoring</u>
			- <u>Logging</u>
## Objectives
---
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
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
	- Occurs when access to computer resources and data <u>happens without consent</u> of the owner ^4eee63
	- Breaking through <u>authorization</u>
- System Failure
	- Computer crashes or an application fails ^1efae6
		- [[Symptoms of Infection]]
	- BSOD
		- Occurs when there is a crash on the PC, indicating a serious issue in #Windows ^e2abc0
		- [[Symptoms of Infection]]
	- Affecting <u>availability</u>
- #SocialEngineering
	- <u>Manipulating user to reveal</u> confidential information or perform action detrimental to user or company ^8a69e4
	- [[Mobile Malware#Phishing|Phishing]]

## Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]

# Mitigating Threats
---
- Physical controls
	- Alarms, locks, cameras, ID cards, guards ^33cf1c
- Technical Controls ^c5223f
	- Smart cards, ACL, [[IDS]], [[NIDS & NIPS]], [[Endpoint Analysis#HIDS/HIPS|HIDS/HIPS]] network authentication ^5453f0
- Administrative Controls ^50e62d
	- AKA "[[Security Controls#Management Controls|Management Controls]]"
	- Policy, procedures, awareness, training, disaster recovery
		- <u>User training one of the most cost effective methods</u>
	- Sub categories
		- Procedural
			- Company policy
		- Legal/Regulatory
			- Adhering to standards and laws
			- PCI, HIPPA,etc…
- See also
	- [[Security Controls#Technical Controls]]
	- [[Security Controls#Administrative Controls]]
## Objectives
---
- [[Objectives#5.1 - Compare and contrast various types of controls|5.1 - Compare and contrast various types of controls]]
- [[Objectives#5.3 - Explain the importance of policies to organizational security|5.3 - Explain the importance of policies to organizational security]]

# Hackers
---
- White Hats ^96bfed
	- Not malicious
	- <u>Work for company</u>
	- "Ethical hackers or Pen Testers"
- Black Hats ^073dd1
	- Bad actors
	- Try to get in without permission or authorization
	- Bad guys
- Grey Hats ^e79201
	- White/Black
	- <u>No affiliation</u>
	- Risk breaking law
	- <u>May not have malicious intent</u>
	- Hacking for the sake of hacking not to cause damage
	- Still breaking the law in general but may responsibly disclose
- Blue Hats ^c8e022
	- Attempting to hack into company at their request
	- <u>Freelancer or contractor</u>
	- Bug bounty
- Elite Hats ^380c86
	- <u>The "best"</u>
	- Find 0 days
	- Create own tools
	- White. Black, Grey hats
	- '1/10,000 considered'
- #Script Kiddies ^5861aa
	- <u>Low level of skill</u> ^87294b
	- Use tools without understanding

## Objectives
---
- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]

# Threat Actors
---
- #Script Kiddies
	- [[#Hackers]] with <u>no/ittle skill or ability</u>
	- "Baby Hackers"
	- Blindly use tool
- Hacktivists
	- [[#Hackers]] <u>driven by cause</u> terrorism, social justice, etc
- Organized crime
	- Group of <u>hackers well-funded</u> and sophisticated
- Advanced Persistent Threats ^f3f779
	- <u>Nation state</u>, covert, uses #OSINT
	- Gain more #Intelligence and info before attacking
	- Often maintain a <u>low profile</u> and <u>persistent access</u>
	- Can take place over longer periods off time
	- Difficult to detect

## Objectives
---
- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]

# Threat #Intelligence and Sources

## Assessing #Intelligence
---
- Weighing value of #Intelligence
	- Timeliness
		- Is it up to date?
		- #Intelligence Less valuable over time
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

## Sources
---
- Proprietary
	- <u>Paid commercial</u> services
	- May not have own data and just aggregate others
- Closed
	- Data <u>derived from their own research</u> from analysis and reports
	- FireEye - Proprietary with closed data
- Open source
	- Data <u>openly available</u> without subscription ^eb8c2e
	- Methods of obtaining Information about a person or organization through public records, websites, and social media ^22bb02
	- Reputation lists and [[Malware]] signature databases
	- US-CERT
		- Computer emergency readiness team
		- Regular reports, analysis, bulletins
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
- Unidirectional Threat Feed
	- One entity produces and shares threat intelligence that others consume, and those consuming the #Intelligence do not contribute in return[^1] ^7137a9
- Bidirectional Threat Feed
	- #Intelligence is sent down to be consumed but can also be ingested from member organizations. Although sharing is allowed and encouraged in these programs, there is no guarantee that every organization will share anything[^1] ^15c875
- Automatic Indicator Sharing ^dd013e
	- An automated way to share indicators of compromise (IOCs) and threat intelligence information ^b5a85f
	- Enables the <u>real-time exchange of machine-readable cyber threat indicators and defensive measures</u> to help protect participants of the AIS community and ultimately reduce the prevalence of cyberattacks[^2]
	- The AIS community includes private sector entities; federal departments and agencies; state, local, tribal, and territorial (SLTT) governments; information sharing and analysis centers (ISACs) and information sharing and analysis organizations (ISAOs); and foreign partners and companies[^2]

## Threat feeds
---
- Threat intelligence from Commercial, Proprietary, and Open Sources
	- Derived from both Explicit Knowledge and Implicit Knowledge
- <u>Explicit knowledge</u>
	- Knowledge you can write down, see, or touch
- <u>Implicit knowledge</u>
	- Experienced practitioners analysis ^b8800d
	- "Sense" what is wrong
	- Ability to have attitude and instinct
	- Can't write down.
		- Purely Experience

## Objectives
---
- [[Objectives#1.5 - Explain different threat actors, vectors, and intelligence sources|1.5 - Explain different threat actors, vectors, and intelligence sources]]
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]

# Threat Hunting
---
- Cyber security technique designed to <u>detect presence of threats not discovered by normal security monitoring</u> ^2a9491
- Is a <u>proactive method vs reactive</u> such as in Incident Response
- Potentially less disrupting than pen test
	- Analyze data within systems you already have access to
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
	- Threat Hunting
		- Using tools for regular security and Incident Response
			- Logs, file, registry changes
			- A #SIEM
		- <u>Assume regular security systems have failed</u>
		- Examine information such as:
			- Network traffic analysis
				- List of suspicious hosts
			- Check executables on hosts
				- Confirm validity of processes
			- Check other hosts
				- Compare similarities
			- Identify how the [[Malware]] or malicious process was executed
- Can consume a lot of resources but can yield some benefits
	- Improve detection capabilities
	- Integrate new info into #Intelligence
		- Corelating external info with internal logs
		- Actionable #Intelligence
	- Reduce attack surface
	- Block [[Malware Infections#Attack Vector|Attack Vector]]
	- Identify critical assets
		- Improve monitoring around those systems

## Objectives
---
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
		- Attackers couple #Payload with #Exploit code
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
	- Command and Control
		- Where weaponized code talks to an outside server to use additional functions ^002bc8
		- Able to remotely use host at this point
		- Establishes 2 way communication
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
	- [[Firewalls]] logs can point to an IP being accessed by several hosts
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

[^1]: https://www.anomali.com/resources/sharing-threat-intelligence
[^2]: https://www.cisa.gov/ais