---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Screens traffic and protects one network from another ^3a1f24
- Most firewalls operate at either [[The OSI Model#Network|Layer 3]] or [[The OSI Model#Transport|Layer 4]]
	- [[#Application Layer Gateway (ALG)]] becoming more popular
	- Other types include [[#Network Address Translation (NAT) Filtering]], [[#Circuit Level Gateway]], and [[#Web Application Firewall (WAF)]]
- See also 
	- [[Unnecessary Ports]]
	- [[Routers#Access Control List (ACL)]]
	- [[#Access Control List (ACL) Config & Rules]]

# Types

## Hardware Firewalls
---
- Standalone physical device or appliance

## Software Firewalls
---
![[Software Firewalls]]

## Embedded Firewalls
---
- A single function on a multifunctional device
- Such as [[Routers]] and [[Unified Threat Management]] systems also including a firewall
- Common in SOHO networks

# Packet Filtering

## About
---
- Firewall inspects each packet passing through the firewall and accepts or rejects it based on the rules
- Such as [[Routers#Access Control List (ACL)|Access Control List (ACL)]]
- Runs either as [[#Stateful]] or [[#Stateless]]

## Stateless
---
- Only analyzes traffic based on IP or ports and makes an 'accept' or 'deny' decision ^efd3f0
- Uses [[Routers#Access Control List (ACL)|Access Control List (ACL)]]

## Stateful
---
- Tracks request that <u>LEAVE</u> through the firewall ^75eecb
- Temporarily open a high number port
- Can almost eliminate IP [[Spoofing]] because each header received is being inspected
- Compares against what it was expecting based on the request that went out
- It then makes an 'accept' or 'deny' decision based on its [[Routers#Access Control List (ACL)|Access Control List (ACL)]]rules
- This makes it more in depth compared to [[#Stateless]]

# [[Network Address Translation]] (NAT) Filtering
---
- Filter traffic based on the ports being used and type of connection such as [[The OSI Model#Transport|UDP]] or [[The OSI Model#Transport|TCP]] ^50150a
- Check endpoint connection by matching incoming traffic to requesting IP and port

# Application Layer Gateway (ALG)
---
- Conducts inspection based on application being used such as [[Defeding the Servers#File Transfer Protocol (FTP) Servers|FTP]] or Telnet ^710136
- Instead of blocking based on ports that are used, it inspects headers to determine the type of application it is meant for
- Resource intensive
- "[[The OSI Model#Application|Layer 7]] firewalls"
- Rising in popularity

# Circuit Level Gateway
---
- Operates at the [[The OSI Model#Session|Session]] layer and <u>only</u> inspects traffic during the <u>establishment</u> of the initial session over [[The OSI Model#Transport|UDP]] or [[The OSI Model#Transport|TCP]] ^5ecc78
- Once established the rest of the traffic can go through without any additional checks

# Web Application Firewall (WAF)
---
- More modern firewall
- Protects your server by inspecting traffic being sent to and from a specific web application ^f3e13f
- Helps prevent [[XSS and XSRF#Cross Site Scripting (XSS)|Cross Site Scripting (XSS)]] and [[SQL Injection]] because they specifically look for threats like these specifically

# MAC Filtering
---
- Stop computers on [[Network Zones#LAN|LAN]] from accessing certain things based on a MAC ^d377c8
- Analyzes/Stops before device and traffic reaches the [[The OSI Model#Network|Network]] layer on any other physical ports

# Access Control List (ACL) Config & Rules

## About
---
- Firewalls will <u>usually read ACL rules in the order</u> of:
	- Type of traffic such as over [[The OSI Model#Transport|UDP]] or [[The OSI Model#Transport|TCP]]
	- IP source
	- IP destination
	- Port
- ACL rules are also processed in the order that is configured starting with 1 and working its way up
	- Once an ACL rule matches the request the firewall made, <u>no additional rules are processed</u>
- See also 
	- [[Routers#Access Control List (ACL)]]

## Rules
---
- Explicit Allow
	- Allowing traffic to enter or leave the network because there is an ACL rule that <u>specifically</u> allows it
	- "allow TCP 10.0.0.2 any port 80"
		- Host with that IP can send packets out to any IP as long as it is over port 80
- Explicit Deny
	- Traffic is denied the ability to enter or leave the network because there is an ACL that <u>specifically</u> denies it
	- "deny TCP any any port 23"
		- Stops any device on the network from sending information over the [[Network Zones#WAN|WAN]] on port 23
- Implicit Deny
	- Traffic denied the ability to enter or leave the network because there is <u>no specific rule</u> that <u>explicitly allows</u> it
	- Create an ACL rule at the bottom of the list (highest number)
	- "deny TCP any any port any"
		- Stops any outbound TCP traffic
	- Common for this to be the default on newer firewalls

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#4.4 - Given an incident, apply mitigation techniques or controls to secure an environment|4.4 - Given an incident, apply mitigation techniques or controls to secure an environment]]

# TODO (Delete when done)
---
- [x] Added vocab
- [x] Added and linked objectives in document
- [x] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document