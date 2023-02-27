---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Bluetooth
	- [[Bluetooth Attacks#BlueJacking|BlueJacking]]
		- <u>SENDS</u> information to a device
	- [[Bluetooth Attacks#BlueSnarfing|BlueSnarfing]]
		- <u>TAKES</u> information form a device
- [[#Radio Frequency Identification (RFID)]]
- [[#Cellular]]
- [[#Near Field Communication (NFC)]]
- [[#Global Positioning System (GPS)]]
- [[#Satellite]]

```ad-tip
title: Exam Tip
collapse: close
- CompTIA almost always has at least one question about [[Bluetooth Attacks#BlueJacking|BlueJacking]] or [[Bluetooth Attacks#BlueSnarfing|BlueSnarfing]]
```

# Radio Frequency Identification (RFID)
---
- Devices that use a radio frequency signal to transmit identifying information about the device or token holder ^1af860
- Can send data from a card to a reader to [[SecBasics#^45fffd|Authentication]] and identification
- Common in Alarm and/or Door Access systems
- Can work from 10 cm to 200 meters
- The larger the distance the more concern there should be about eavesdropping or a [[Replay Attack]]

# Near Field Communication (NFC)
---
- Allows two devices to transmit information when they are within close range through automated pairing and transmission ^b9fdff
- Usually within 4cm
- Information can be replayed or rebroadcasted but with the very short range the risk is low
- Examples
	- Some cell phones can share photos this way
	- Debit/Credit card payment terminals
- See also
	- [[Hardening Mobile Devices]]

# Cellular
---
- 3G, 4G, LTE, 5G, are cellular connection's ^11df4a
- Preferable to use this instead of WIFI since it is a direct connection to a cell tower
- While devices for cellular interception exist they are usually only used at a nation state or law enforcement level

# Global Positioning System (GPS)

## About
---
- A system that offers the ability to obtain positioning, navigation, and timing (PNT) services ^ee7213
- Can be used for
	- [[#Geolocation]]
	- [[#Geotagging]]
	- [[#Geofencing]]
- Typically considered a [[Bring Your Own Device (BYOD)]] concern

## Geolocation

### About
---
- Method of determining the physical location of the user trying to authenticate ^17f818
- Often used in the implementation of mobile device policies, where users are only allowed to access a network based on the location they are reaching the Internet from
	- Can be used in combination with [[#Geofencing]]

### Concerns
---
- GPS device relies on ability to talk to at least 3 of 24 satellites to calculate a position
- The signal from a satellite to device is relatively weak so an attacker could broadcast a more powerful signal from nearby and disrupt communications
- If your organization is relying on GPS for tracking, it should not rely <u>SOLELY</u> on it
	- Have redundancy

## Geotagging

### About
---
- Adding of data to the content in question, helping users to gather location-specific information
- Example
	- Taking a picture with your phone and adding metadata to the photo indicating the location where it was taken
	- Usually a transparent operation that happens without the users intervention
- See also
	- [[Security of Apps#Geotagging]]

### Concerns
---
- Geotagging can be a security concern because it could allow a person to be tracked if an attacker could obtain geotagged information

## Geofencing
---
- The use of a virtual fence defining the boundaries of an actual geographical area ^560563
- Examples
	- Used as a way to be alerted to users entering and exiting an organization’s physical premises
	- Provide security for wireless networks by defining the physical borders and allowing or disallowing access based on the physical location of the user, or more accurately, the user’s computer or mobile device

# Satellite

## About
---
- Used for long distance communication over large distances where other networks are not present ^bac8ef
- Can interconnect two networks or be used as your internet connection
- Example
	- High mountain
	- Merchant ships
- Rare to be relied on for most organization

## Concerns
---
- Can be subject to [[Wireless Access Points (WAP)#Jamming|Jamming]], interception, and [[Securing Network Media#Radio Frequency Interference (RFI)|Interference]] since it is over the air
- Always encrypt data when possible

# Objectives
---
- [[Objectives#1.4 - Given a scenario, analyze potential indicators associated with network attacks|1.4 - Given a scenario, analyze potential indicators associated with network attacks]]
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]
- [[Objectives#3.7 - Given a scenario, implement identity and account management controls|3.7 - Given a scenario, implement identity and account management controls]]