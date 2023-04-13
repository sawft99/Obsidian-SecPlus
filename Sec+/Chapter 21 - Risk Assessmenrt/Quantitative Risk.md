---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Measures [[Risk Assessments#Risk|Risk]] by using exact monetary values ^809030
- It attempts to give an expected yearly loss in dollars for any given risk
- Provides a Magnitude of Impact ^558a48
	- An estimation of the amount of damage that a negative [[Risk Assessments#Risk|Risk]] might achieve ^ef1332
- Grading scale goes from low to high corelating with the cost an organization could face
- Gives a clearer understanding than [[Qualitative Risk]]
- Methods to measure
	- [[#Single Loss Expectancy (SLE)]]
	- [[#Annualized Rate of Occurrence (ARO)]]
	- [[#Annualized Loss Expectancy (ALE)]]
- Opposite of [[Qualitative Risk]]
- In reality a hybrid method of [[Qualitative Risk]] and Quantitative are used
- See also
	- [[Risk Assessments]]

# Single Loss Expectancy (SLE) 
---
- Cost associated with the realization with each individualized [[Risk Assessments#Threats|Threat]] that occurs ^4dde44
- Asset Value x Exposure Factor
	- SLE = AV x EF
- Exposure factor is the amount of the asset that will be lost if the threat is realized
- Example
	- $10,000 server and a threat of power failure that would reduce the functionality down to 20%
	- SLE = 10,000 * 20%
	- $2,000

# Annualized Rate of Occurrence (ARO)
---
- Number of times per year a [[Risk Assessments#Threats|Threat]] is realized ^66d9ba

# Annualized Loss Expectancy (ALE)
---
- Expected cost of a realized [[Risk Assessments#Threats|Threat]] over a given year ^709a90
- ALE = [[#Single Loss Expectancy (SLE)|SLE]] x [[#Annualized Rate of Occurrence (ARO)|ARO]]
- Example
	- $2,000 figure from [[#Single Loss Expectancy (SLE)|SLE]] example
	- [[#Annualized Rate of Occurrence (ARO)|ARO]] incident can happen 3 times a year
	- ALE = 2,000 x 3
	- $6,000

# Decisions
---
- [[#Annualized Loss Expectancy (ALE)]] is used as part of the final decision in what resources are dedicated to a project
- Easier to compare numbers than a subjective value from [[Qualitative Risk]]
- Easier to justify to management that makes decisions
- Example
	- Add up all of the construction and equipment costs which makes the server room come to $200,000
		- It includes measures to address possible power failures used in previous examples
	- You weigh this investment against the risk you are offsetting from the [[#Annualized Loss Expectancy (ALE)|ALE]] 
	- Using the $2,000 figure from the [[#Annualized Loss Expectancy (ALE)|ALE]] example, it would take nearly 33 years to make up for your $200,000 capital expenditure

# Objectives
---
- [[Objectives#5.4 - Summarize risk management processes and concepts|5.4 - Summarize risk management processes and concepts]]