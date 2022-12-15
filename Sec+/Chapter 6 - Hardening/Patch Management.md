---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Patch Management
	- Process of testing, implementing, and auditing of software [[Updates and Patches]] ^f08696
	- Keeps track of all patches for hard and software across organization
	- Also implemented to make sure new patches don't introduce new bugs or issues

# Stages
---
1. Planning
	1. Create policy, systems, and procedures to track updates along with a method to verify that they are compatible
	2. Also determine how to apply
	3. Baseline Security Analyzer (MBSA)
		1. Microsoft tool that helps identify misconfigurations on #Windows  workstations ^974484
2. Testing
	1. Test [[Updates and Patches]] before applying to new network
	2. Create small test network/lab
3. Implementing
	1. Deploy to all workstations that need the patch
	2. Can be automated or manual
		1. System Center Security Configuration Manager (SCCM)
			1. Microsoft tool to help with larger scale patch management ^d1d9c8
		2. Many #Linux OS uses <u>packet managers</u> instead
	3. Larger companies are recommended to use a centrally managed system and not default #Windows  update utility
		4. May want to [[Restricting Applications#CLI|stop Windows Update service]] so 3rd party patch will take over without conflict
	4. If you have mobile devices you may want to handle patch management through [[Security of Apps#Mobile Device Management (MDM)|Mobile Device Management (MDM)]]
4. Auditing
	1. Make sure patch was installed properly and no errors occurred
		1. A tool such as SCCM or another 3rd party tool

# Objectives
---
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]

# TODO (Delete when done)
---
- [x] Added vocab
- [x] Added and linked objectives in document
- [x] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document