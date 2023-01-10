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
- More on XML [Here](https://www.educba.com/xml-encoding/)

```ad-tip
title: Exam Tip
collapse: close
1. Generally if you see any question in regards to XML it is likely related to [[XML Vulnerabilities]]
2. However, be sure it is not HTML or JavaScript since they look similar

| Language   | Give aways                                            |
| ---------- | ----------------------------------------------------- |
| HTML       | font, css, img, or  href                              |
| JavaScript | Some form of scripting, variables, functions, methods |
| XML        | Question, ID, Type, Element, Entity                   |

```

# XML Document Example

## Example Code
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

## Breakdown By Line
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
- Begin document with the XML info line:   ```<?xml version="1.0" encoding="UTF-8"?>```
	- XML version or encoding could be different
	- Last line of document may not need to end with ```</xml>```
- Format anything you define with ```<thing>``` and end with ```</thing>```
- Indent parent/child information for readability
	- Such as above where the document is defined, followed by the question, followed by the questions information and the pattern repeats backwards as you end each definition

# Attacks

## XML Bomb (Billion Laughs Attack)
---
- XML encodes entities he expand to exponential sizes, consuming memory on the host, and potentially crashing it ^fd20be
- Form of #DDoS

## XML External Entity (XXE)

### About
---
- An XML attack that embeds a request for a local resource ^a3ddab
- Similar to File Inclusion
- Attempts to access "file:///etc/shadow" are a giveaway to this type of attack
- To prevent have proper [[SDLC Principles#Never Trust User Input|Input Validation]]

### Example Code
---
```XML
<?xml version="1.0" encoding="ISO-8859-1"?>
	<!DOCTYPE foo [
		<!ELEMENT for ANY >
		<!ENTITY xxe SYSTEM "file:///etc/shadow" >]>
	<foo>&xxe;</foo>
```

## XPath Injection

### About
---
- XPath Injection is an attack technique used to exploit web sites that construct <u>XPath queries from user-supplied input</u>
- By sending <u>intentionally malformed information</u> into the web site, an attacker can find out how the XML data is structured, or access data that they may not normally have access to
- Similar to [[SQL Injection]]

```ad-danger
title: Exam Tip
collapse:open
Xpath questions should not be on the exam but they may use other questions that are based around the URL being changed to accomplish an attack
```

## Example Code
---
```URL
https://mysite.com/add_to_cart.php?itemId=5"+perItemPrice="0.00"+quantity="100"+/><item+id="5&quantity=0
```

## Breakdown
---
- Some XML injection attacks done on a website will send an altered URL
- As seen in the URL above, the attacker is attempting add 100 of "Item 5" for a price of $0 by manipulating user input for an XML field

## Example Video
---

![](https://www.youtube.com/watch?v=xFDI_2nQcz8)


![](https://www.youtube.com/watch?v=6tV8EuaHI9M)

# Objectives
---
- [[Objectives#1.3 - Given a scenario, analyze potential indicators associated with application attacks|1.3 - Given a scenario, analyze potential indicators associated with application attacks]]