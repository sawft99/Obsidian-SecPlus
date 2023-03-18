---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A framework that provides authorization to a third-party entity, such as an application, to access resources hosted on a [[#^061a80|Resource Server]]
- Main feature of OAuth is providing the third party authorization to access restricted resources <u>without passing the client credentials </u>to this third party
- Instead of getting the user credentials, the entity requesting access receives an <u>authorization token</u> that includes authorization information, such as scope and duration, and that is used to request access to a resource hosted by the [[#^061a80|Resource Server]]
- See also
	- [[Authentication Models]]
	- [[OpenID Cont.]]

# Roles
---
- Resource owner
	- The party that owns the resource (for example, a user) and grants authorization to access some of its resources
	- Comparable to [[Authentication Models#^d513a9|Principal/Subject]] 
- Client
	- The party that requires access to a specific resource
	- Such as a mobile phone or browser
- Resource server ^061a80
	- The party that hosts or stores the resource
	- Comparable to [[Authentication Models#^8af39b|Service Provider]]
- Authorization server
	- The party that provides an authorization token
	- Comparable to [[Authentication Models#^5e1700|Identity Provider]]

# Process
---
1. The client sends an authorization request to the resource owner or indirectly to the authorization server
2. The resource owner (or the authorization server on behalf of the resource owner) sends an authorization grant to the client
3. The client sends the authorization grant to the authorization server as proof that authorization was granted
4. The authorization server authenticates the client and sends an access token
5. The client sends the access token to the resource server as proof of authentication and authorization to access the resources
6. The resource server validates the access token and grants access

```ad-example
title: OAUTH Exchange
collapse:close
![[OAUTHEx1.png]]
```

# Objectives
---
- Obj

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document