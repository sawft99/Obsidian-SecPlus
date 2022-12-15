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
		1. Microsoft tool
		2. Helps identify misconfigurations on #Windows  workstations
2. Testing
	1. Test [[Updates and Patches]] before applying to new network
	2. Create small test network/lab
3. Implementing
	1. Deploy to all workstations that need the patch
	2. Can be automated or manual
	3. System Center Security Configuration Manager (SCCM)
		1. Microsoft tool to help with larger scale patch management
	4. Larger companies are recommended to use a centrally managed system and not default #Windows  update utility
		1. May want to [[Restricting Applications#CLI|stop Windows Update service]] so 3rd party patch will take over without conflict
4. Auditing


# Objectives
---
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document