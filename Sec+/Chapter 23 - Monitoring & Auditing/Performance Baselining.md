---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Process of measuring changes in networking, hardware, software, or applications ^a1ee0f
- See what normal is and then measure against to see what is abnormal
- By defining the baseline you can then perform Baseline Reporting
	- Documenting and reporting changes in the baseline ^c78209
- In addition to establishing a baseline of the current environment you also have a baseline for a system you are creating
	- This is part of your [[#Security Posture]]

# Security Posture
---
- [[Risk Assessments#Risk|Risk]] level to which a system or other technology element is exposed ^f4264d
- Tied to to concepts of configuration management, patch levels, programs installed and configuration of a system
- Synonymous with meeting your acceptable [[Risk Assessments#Risk|Risk]]
- If you want a lower of level of risk then you want to heavily control all aspects of it [[Risk Assessments#Risk|Risk]]

# Performance
---
- Measuring bandwidth, disk space, CPU usage overall operations and functionality
- Important in security a since performance impacts may be one of the [[Symptoms of Infection]]
- Common utility in #Windows is perfmon.exe
	- Not helpful in real time
	- Instead configuring alerting with other software if certain thresholds are met

```ad-example
title: Perfrmon
collapse:close
![[PerfmonEx1.png]]
```

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]