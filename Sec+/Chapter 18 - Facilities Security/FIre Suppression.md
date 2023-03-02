---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Process of controlling and/or extinguishing fires to protect an organization's employees, data, equipment, and [[Physical Security#Building|Buildings]] ^9f1d91
- Types of fires
	- [[#Class A]]
	- [[#Class B]]
	- [[#Class C]]
	- [[#Class D]]
	- [[#Class K]]
- Types of suppression
	- [[#Handheld]]
	- [[#Sprinklers]]
	- Special Hazzard Protection
		- [[#Clean Agent System]]

# Types of Fires

## About
---
- Not all fires are the same
- Fire types
	- [[#Class A]]
	- [[#Class B]]
	- [[#Class C]]
	- [[#Class D]]
	- [[#Class K]]

## Class A
---
- <u>Solid combustible materials</u>
	- Wood, paper, etc
- A water based extinguisher
- Shouldn't use in a data center, server room, or on other electronic equipment since water may damage it

```ad-example
title: Class A Extinguisher Symbols
collapse:close
![[ExtinguisherHandheldAEx1.png]]
```

## Class B
---
- For <u>flammable gasses or liquids</u>
- Should use dry chemical agent or CO2 based extinguisher

```ad-example
title: Class B Extinguisher Symbols
collapse:close
![[HandheldExtinguisherBEx1.png]]
```

## Class C
---
- For <u>electrical equipment</u>
- First try to shut off power since this may stop the fire if the electricity is the source
- CO2 extinguisher is also good for this

```ad-example
title: Class C Extinguisher Symbols
collapse:close
![[HandheldExtinguisherCEx1.png]]
```

## Class D
---
- For <u>combustible metals</u>
	- Magnesium, Titanium, Lithium
- Laptops have Lithium batteries

```ad-example
title: Class D Extinguisher Symbols
collapse:close
![[HandheldExtinguisherDEx1.png]]
```

## Class K
---
- For <u>cooking oils</u>
	- Grease oil
- Have in kitchen

```ad-example
title: Class K Extinguisher Symbols
collapse:close
![[HandheldExtinguisherKEx1.png]]
```

# Extinguisher Types

## About
---
- Types
	- [[#ABC Extinguishers]]
	- [[#BC Extinguishers]]
	- [[#D Extinguishers]]

## ABC Extinguishers
---
- Good for fires of
	- [[#Class A]]
	- [[#Class B]]
	- [[#Class C]]
- Uses dry chemicals
- Avoid if possible for [[#Class C]] fires though as the chemicals are <u>corrosive to computers</u> and some other electrical parts 

```ad-example
title: ABC Extinguisher
collapse:close
![[ABCExtinguisherEx1.png]]
```

## BC Extinguishers
---
- Most common type
- Also call a "CO2 Extinguisher"
- Used for [[#Class B]] and [[#Class C]] types of fires
- <u>Better for computers</u> and other electrical parts as it does not have a corrosive chemical
- Smothers fires with CO2 so people nearby may have a hard time breathing

```ad-example
title: BC Extinguisher
collapse:close
![[BCExtinguisherEx1.png]]
```

## D Extinguishers
---
- Less common
- <u>Typically yellow</u>
- Used for [[#Class D]] fires

```ad-example
title: D Extinguisher
collapse:close
![[DExtinguisherEx1.png]]
```

# Sprinklers

## About
---
- In celling and pipes above area
- Types
	- [[#Wet]]
	- [[#Dry]]
	- [[#Pre-Action]]
- Typically not a good choice to have in a server room since it uses water
- Have red bulbs in them that when melted or broken trigger a [[#Wet]] or [[#Dry]] sprinkler system

```ad-example
title: Sprinkler System Head
collapse:close
![[SprinklerSystemEx1.png]]
```

## Wet
---
- Pipes are already filled with water all the way to the sprinkler head and wait for the red glass bulb to be melted or broken ^d9fa4b
- If in a cold environment there is a <u>potential to freeze or crack the pipes</u> since water sits inside of the pipes at all times

## Dry
---
- Pipes are filled with pressurized air and only push water into the pipes once the red glass bulb is melted or broken ^020cda

## Pre-Action
---
- Like a [[#Dry]] pipe solution, but is triggered when heat or smoke is detected ^1d52b4
- <u>WILL NOT</u> trigger when red bulb is melted or broken, smoke and/or heat also needs to be detected

# Clean Agent System
---
- Fire suppression system that relies upon gas (HALON, FM-200, or CO2) instead of water to extinguish in a fire ^a29c83
- HALON less common now as it is bad for the environment
- If you hear a fire alarm in a server room that has this system <u>RUN</u>!
	- Gas will suffocate the fire <u>AND you</u>

# Objectives
---
- [[Objectives#2.7 - Explain the importance of physical security controls|2.7 - Explain the importance of physical security controls]]