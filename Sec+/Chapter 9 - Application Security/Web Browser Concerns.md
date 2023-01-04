---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Additional considerations for [[Web Browser Security]]

# Cookies
---
- Text files placed on a clients computer to store information about the user's browsing habits, credentials, and other data ^d06d5f
	- Website authentication, session tracking, shopping carts
- Types
	- Tracking
		- Often used by [[Spyware]]
		- Learn what websites you go to, how long you use, what you click on, etc
	- Session
		- Keeps track of user, preferences, shopping cart, etc
		- Maintains connection/session between you and the server
- Secure Attribute
	- When a cookie has the Secure attribute, the user agent includes the cookie in an HTTP request <u>only if the request is transmitted over a secure channel</u> (typically HTTPS).
	- Although seemingly useful for protecting cookies from active network attackers, the Secure attribute <u>protects only the cookie’s confidentiality</u>
	- Forcing the web application to use TLS or SSL <u>does not force</u> the cookie to be sent over TLS/SSL, so you still would need to set the Secure attribute on the cookie.
	- Hashing the cookie provides <u>integrity of the cookie, not confidentiality</u>.
- Cookies are becoming blocked or removed now, some companies have moved to "Server side tracking"
	- Allows them to do similar tracking without cookies

# Locally Shared Object (LSO)
---
- Cookies stored in #Windows user profile under the Flash folder inside of your AppData Roaming folder ^30b780
- Aka "Flash Cookies"
- <u>Flash is being phased out in favor of HTML5</u>
- Can be disabled in Flash Player settings or in local settings manager

# Add-Ons
---
- Smaller browser extensions and plugins that provide additional functionality to the browser ^4017f6
- Examples
	- Adobe Flash or Shockwave
	- Password manager
- Not necessarily bad but it can introduce additional code which can bring vulnerabilities
- Could also download add-ons from outside the normal stores where they can more likely to contain [[Malware]]
- Organizations will often block additional [[#Add-Ons]] to keep the browser "slim"
	- See also [[Unnecessary Applications]]

# Advanced Security Options
---
- Browser configuration and settings for numerous options such as SSL/TLS settings, local storage/cache size, browsing history, and more ^3759d6
- All browsers have settings that can be configured for the security settings

# Configuring the Browser - Examples

## Home Users - IE 11
---
```ad-example
title: Internet Options
collapse:close
1. First go to Internet Options
![[Windows_IEOptions1.png]]
```

```ad-example
title: Home Page & History
collapse:close
2. Confirm Home Page and History settings
![[Windows_IEOptions2.png]]
![[Windows_IEOptions3.png]]
```

```ad-example
title: Security Zones
collapse:close
3. Configure security settings of zones and add sites, if needed, to the various lists
![[Windows_IEOptions4.png]]
```

```ad-example
title: Popups
collapse:close
4. Confure the popup blocker and any allowed sites
![[Windows_IEOptions5.png]]
![[Windows_IEOptions6.png]]
```

```ad-example
title: Cookies
collapse:close
5. Configure cookie settings
![[Windows_IEOptions7.png]]
```

```ad-example
title: AutoComplete
collapse:close
6. Configure any autocomplete settings
![[Windows_IEOptions8.png]]
![[Windows_IEOptions9.png]]
```

```ad-example
title: Proxy
collapse:close
7. Configure Proxy settings
![[Windows_IEOptions10.png]]
![[Windows_IEOptions11.png]]
```

```ad-example
title: Advanced
collapse:close
8. Many more settings can be configured from the advanced menu
![[Windows_IEOptions12.png]]
```

## Enterprise - IE 11
---
```ad-example
title: Locate Group Policy Section
collapse:close
1. Administrative Templates > WIndows Components > Internet Explorer
![[Windows_GPOIE1.png]]
```

```ad-example
title: Configure Settings
collapse:close
2. Configure Settings as Needed
![[Windows_GPOIE2.png]]
```

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]