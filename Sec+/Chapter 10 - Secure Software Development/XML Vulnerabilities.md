---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Extensible Markup Language (XML)
	- A programming language used for authentication, authorization, and other types of data exchange or uploads ^5a1e86
- May be referred to as an "XML Injection" but this is not technically correct as the vulnerabilities lie in parsing
- XML data is submitted from you to the server or from server to server
- So make sure there is encryption and [[SDLC Principles#Never Trust User Input|Input Validation]] otherwise it can be vulnerable to #spoofing, [[XSS and XSRF#Cross Site Request Forgery (XSRF/CSRF)|Request Forgery]] and [[SQL Injection#Injection Attack|Injection]] of arbitrary code

# Format Example

## Code
---
```XML
<?xml version="1.0" encoding="UTF-8"?>
	<question>
		<id>CYSA-002-0001<id>
		<title>Is this an XML vulnerability? </title>
		<choice1>Yes</choice1>
		<choice2>No</choice2>
	</question>
</xml>
```

## Breakdown
---
1. Specifies the version of XML and the encoding used
2. Defines a question
3. An ID for the question
4. The title of the question
5. Representing a choice to select
6. Representing a choice to select
7. Closing/Ending definition of question
8. Closing/Ending the xml document

## Always
---
- Begin document with the XML info line ```<?xml version="1.0" encoding="UTF-8"?> ``` and end with ```</xml>```
	- XML version or encoding could be different
- Format anything you define with ```<thing>``` and end with ```</thing>```
- Indent parent/child information for readability
	- Such as above where the document is defined, followed by the question, followed by the questions information and the pattern repeats backwards as you end each definition
s
# Attacks

## XML Bomb (Billion Laughs Attack)
---
-

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document