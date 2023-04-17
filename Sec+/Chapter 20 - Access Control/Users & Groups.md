---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Relies on subjects and objects
- Subjects being <u>users or people</u>
- Objects can be <u>things</u> like files, folders, devices, computer or groups of users
	- Groups can contain other groups
	- Easier using groups to manage user permissions
	- An important part of [[Access Control#Role Based Access Control (RBAC)|Role Based Access Control (RBAC)]]

# Active Directory Users and Computers  (ADUC)

## About
---
- Used to manage users and groups in a #Microsoft #Windows environment
- See also
	- [[Group Policies#Active Directory]]

## Methods

### Method 1
---
1. Right click an empty area in the "Users" folder of ADUC 
2. Select "Create New User"
- Typically for small companies or setups

```ad-example
title: ADUC
collapse:close
![[ActiveDirectoryEx1.png]]
```

### Method 2 - Large company/setup
---
1. Create a new user in an Organizational Unit (OU)
- Typical for larger companies or setups
	- More common in general
- Often OUs coincide to departments such as IT, HR, Marketing, etc

```ad-example
title: ADUC w/ OU
collapse:close
![[ActiveDirectoryEx2.png]]
```

# User Rights
---
- Whatever permissions are assigned to a given user ^147b51
- Not just file permissions but also logon abilities, account expiration, how often to change a password, what printers can be used  and more

```ad-example
title: User properties
collapse:close
![[ADUserPropertiesEx1.png]]
```

```ad-example
title: Logon Hours
collapse:close
- You may want to constrict logon hours to business hours so a user can't potentially do somethinh they shouldn't when no one is around
![[ADUserPropertiesEx2.png]]
```

# Groups
---
- Collection of Users based on common general attributes such as roles

```ad-example
title: Folder Permissions
collapse:close
![[FolderPermEx1.png]]
```

# Permissions in Windows
---
- Full Control
- Modify
- Read & Execute
- List Folder Contents
- Read
- Write

# Permissions in Linux
---
- Read
- Write
- Execute

# Groups in Linux
---
- Owners (U)
- Groups (G)
- All Users (O/A)

# Modify Permissions in Linux
---
- chmod
	- Program that is used to change the permissions or rights of a file or folder with a shorthand numbering system
	- (R) Read - 4
	- (W) Write - 2
	- (X) Execute - 1
- Can be combined
- Example
	- Bob with a value of 7
	- Means he can Read and Write
- Usually supply 3 separate digits to indicate the level of access for the Owner, Group, and All Users
- Example
	- chmod 760 filename
	- 7 = Owner (RWX)
	- 6 = Group (RW)
	- 0 = All Users (No access)

# Privilege Creep
---
- Occurs when a user gets additional permission over time or as they rotate through different positions or roles ^4c62f5
- This violates the principle of [[SDLC Principles#Least Privilege|Least Privilege]]

# User Access Recertification
---
- Process where each users permissions are revalidated to ensure they are correct ^41017d
- Can be done manually or through an automated process
- Helps address [[#Privilege Creep]]
- There are 3 times that a users permissions should/will change; hiring firing, and promotion
- Recertification should happen at each stage

# Objectives
---
- [[Objectives#3.7 - Given a scenario, implement identity and account management controls|3.7 - Given a scenario, implement identity and account management controls]]
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]
- [[Objectives#4.1 - Given a scenario, use the appropriate tool to assess organizational security|4.1 - Given a scenario, use the appropriate tool to assess organizational security]]