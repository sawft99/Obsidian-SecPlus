---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Determine what file system you should use and how it will affect [[Hardening]] your computer
- Types
	- New technology File System (NTFS)
	- File Allocation Table (FAT32)
	- Extended File System (ext4)
	- HFS+
	-  Apple file System (APFS)
- Use [[Disk Encryption#Full Disk Encryption|Full Disk Encryption]] when possible

# Platforms

## #Windows
---
- Can utilize FAT32 or NTFS
- NTFS
	- The default file system format for #Windows and is more secure because it supports logging, [[Securing Storage#Encryption|Encryption]]/[[Disk Encryption]], larger partition sizes, and larger files than FAT32
	- Is newer and <u>recommended to use</u> over FAT32
	- Can convert FAT32 to NTFS
		- 'Convert DriveLetter:\ /FS:NTFS'

## #Linux
---
- Uses ext4

## #OSX
---
- Should use APFS
	- The most recent and most secure version support on #OSX

# Maintenance and Recovery

## About
---
- Hard drives eventually fail so there are methods to extend the life and help with recovery

## Methods
---
1. Remove temporary files
2. Conduct periodic file system checks
	1. #Windows - chkdsk
	2. #Linux  - fsck
	3. #OSX - "First Aid" in disk utility app
3. Defrag
	1. Defrag via cli or app
4. Ensure good backups
	1. Multiple software and cloud solutions
5. Know how to use restore techniques and verify your backups
	1. System restore points
	2. Tape backups
	3. Hard drive backups
	4. Individual backups

## Examples
---
### File System

```ad-info
title: Windows - chkdsk
collapse:close
![[Win_FS_chkdsk.png]]
```

```ad-info
title: Linux - fsck
collapse:close
![[Linux_fsck.png]]
```

```ad-info
title: OSX - First Aid
collapse:close
![[OSX_FistAid.png]]
```

### Defrag

```ad-info
title: Windows - Defrag CLI
collapse:close
![[Win_Defrag_CLI.png]]
```

```ad-info
title: Windows - Defrag App 
collapse:close
![[Win_Defrag_App.png]]]
```

```ad-info
title: OSX - Defrag App
collapse:close
![[OSX_Defrag_App.png]]
```

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document