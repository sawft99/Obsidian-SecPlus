---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Methods used to secure data and information (including physical controls) by verifying a user has permission to access, read, write, delete or modify it in some other way ^f9403b
- Comprised of several different models
- See also
	- [[As a Service#Other Cloud Services]]

# Discretionary Access Control (DAC)
---
- The access control policy is determined <u>by the owner</u> ^eea57c
- An object can be a file, folder, network connection, or device ^fa3911
- A single user can be an owner
- A common method
- Granular
- Caveats
	- Every object in a system must have an owner
		- Otherwise something could be openly accessible by anyone or anything
	- Each owner determines access right permissions for each object
		- Can be made too lose or too tight

# Mandatory Access Control (MAC)

## About
---
- An access control policy where <u>the computer system</u> determines the access control for an [[#^fa3911|object]] ^c000ea
- The opposite of [[#Discretionary Access Control (DAC)]]
- Uses [[#Data Labels]] to determine access
- Considered the <u>most strict</u> and is usually in <u>high security environments</u>
- Implemented as either [[#Rule Based]] or [[#Lattice Based]] 
- Exists in FreeBSD & SELinux and not #Windows

## Data Labels
---
- Creates a trust level for all [[Authentication Models#^d0e955|subject]] and [[#^fa3911|objects]] such as high, medium, and low trust ^e69c2f
- Common in a very high security environment such as with government documents
	- Unclassified
	- Confidential
	- Secret
	- Top secret
- These labels apply to both the level of access a person has as well as the classification for the document
	- For example, a document being labeled 'top secret' and a certain person in the military only allowed <u>up to</u> the 'confidential' level of access
- There is also a 'need to know' element meaning that even if you have access up to that level, it may not be something pertaining to you
	- For example, a person in the Army with 'top secret' clearance may not be able to access a Navy 'top secret' document

## Rule Based
---
- Label based access control system that defines whether access should be granted or denied to objects by comparing the object label and the subject label
- For example, your level of access is 'confidential' and the document is labeled as 'confidential' so you are granted access 

## Lattice Based
---
- Uses complex mathematics to create sets of [[#^fa3911|objects]] ad [[Authentication Models#^d0e955|subjects]] to define how they interact
- This attempts to go after the 'need to know' factor

# Role Based Access Control (RBAC)
---
- An access model that is controlled by the system (like [[#Mandatory Access Control (MAC)|MAC]]) but utilizes a <u>set of permissions applied to a group</u> instead of a single [[#Data Labels|Data Label]] to define the permission level
- For example, roles for HR, Sales, Marketing, IT, etc
- You then add or remove people from these roles rather than changing permissions for every file and folder
- See this in #Windows [[Group Policies#Active Directory|Active Directory]]

# Attribute Based Access Control (ABAC)
---
- An access model that is <u>dynamic and context-aware</u> using IF-THEN statements
- Uses multiple policies that can combine various user, group, and resource attributes together to form a complete picture
- <u>Newer</u> form of Access Control
- For example
	- IF Jason is in HR THEN give him access to \\\\fileserver\\HR

# Conditional Access
---
- An access control model where access is granted based on <u>specific criteria</u> requirements such as IP address, type of browser, type of operating system, or geographic location
- Primarily in [[As a Service#Software as a Service (SaaS)|Software as a Service (SaaS)]]

# Privilege Access Management (PAM)
---
- An access control system used to centrally manage access to privileged accounts
- Identifies the people, processes, and technology that require privileged access and specifies the policies that apply to them [^1]
- [[SDLC Principles#Least Privilege|Least Privilege]] concept applied
- Mostly used to securely <u>store the elevated credentials</u> used by an organization and <u>broker the use</u> of those credentials based on <u>criteria</u> set by a privileged access management administrator

# Objectives
---
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]

[^1]: https://www.microsoft.com/en-us/security/business/security-101/what-is-privileged-access-management-pam