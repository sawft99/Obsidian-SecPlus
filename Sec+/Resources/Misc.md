---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# [[Cloud Based Infrastructure]]
---
- Vendor Lock In ^d2ea95
	- Because of cost or another serious limitation you can be "forced" to stay with a vendor ^2f2cac
	- For example, you have a large amount of data and attempting to move to another provider could incur large expenses because of bandwidth or storage costs that would be required to migrate
-  On Premise pro
	- In your data center with physical access ^851f11
		- Ensures you maintain your [[SecBasics#^51b6d8|CIA]] and [[SecBasics#^45fffd|AAA]] security models

# ICS, SCADA, Premise System, Etc. Difference


```mermaid
flowchart LR
  
subgraph ES[Embedded Systems]
	HVAC
end
subgraph OpTec[Operational Technology]
	FB[FieldBus]
	MoBu[ModBus]
	subgraph ICS
		SCADA
		HMI[Human Machine Interface]
		DaHi[Data Historian]
		PLC[PLC/SOC]
	end
end
subgraph PS[Premise Systems]
	subgraph PACS[Physical Access Controls]
		Cameras
		DoLok[Door Lock]
	end
	BAS[Building Automation Systems]
end

ICS -- Manages --> ES
SCADA -- Manages multiple over WAN --> PLC
BAS -- Can incorporate --> HVAC
PLC -- Manages --> ES
ES -- Runs for an OS --> RTOS
HMI -- Controls --> PLC
DaHi -- Collects Info --> SCADA
DaHi -- Collects Info --> PLC
BAS -- Can incorporate --> PACS
```

# ICS MAP1

![[#ICS, SCADA, Premise System, etc. Difference]]

# Inter ICS Comms

```mermaid
flowchart TD

subgraph OT[Operational Technology]
	MoBu[ModBus]
	FiBu[FieldBus]
	subgraph ICS
		direction TB
		PLC[PLC/SOC]
		SCADA
	end
end
SCADA <-.-> MoBu
MoBu <-.-> PLC
PLC <-.-> FiBu 
FiBu <-.-> PLC
```

# ICS MAP2

![[#Inter ICS Comms]]

# IOT and ICS Grouping

```mermaid
flowchart TD
subgraph IOT
	subgraph ES[Embeded Systems]
		HVAC
	end
	subgraph PS[Premise System]
		subgraph BAS[Building Automation Systems]
		end
		subgraph PACS[Physical Access Controls]
		end
	end
	subgraph OT[Operational Technology]
		direction RL
		FiBu[FieldBus]
		MoBu[ModBus]
		subgraph ICS
			direction LR
			HuMi[Human Machine Interface]
			SCADA
			PLC[PLC/SOC]
			DaHi[Data Historian]
		end
	end
end

```

# ICS Map3
---
![[#IOT and ICS Grouping]]


- Ref
	- [Flowchart](https://mermaid.js.org/syntax/flowchart.html)
	- [Sequence](https://mermaid.js.org/syntax/sequenceDiagram.html)
	- [Journey](https://mermaid.js.org/syntax/userJourney.html)
	- [Pie](https://mermaid.js.org/syntax/pie.html)
	- [GitGraph](https://mermaid.js.org/syntax/gitgraph.html)
	- [Timeline](https://mermaid.js.org/syntax/timeline.html)