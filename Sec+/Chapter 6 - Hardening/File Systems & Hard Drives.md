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
	- Extended File System (ext4) ^8e18e9
	- Hierarchical File System+ (HFS+) ^729b3d
	-  Apple file System (APFS) ^5736b2
- Use [[Disk Encryption#Full Disk Encryption|Full Disk Encryption]] when possible

# Platforms

## #Windows
---
- Uses FAT32 or NTFS
- NTFS
	- The default file system format for #Windows and is more secure because it supports logging, [[Disk Encryption#Full Disk Encryption|Full Disk Encryption]], larger partition sizes, and larger files than FAT32 ^ada5d0
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
- HFS+ was replaced by APFS
- HFS was replaced by HFS+

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
4. Backups
	1. Multiple software and cloud solutions
5. Know how to use restore techniques and verify your backups
	1. System restore points
	2. Tape backups
	3. Hard drive backups
	4. Individual backups

## Examples
---
### File System

```ad-example
title: Windows - chkdsk
collapse:close
![[Win_FS_chkdsk.png]]
```

```ad-example
title: Linux - fsck
collapse:close
![[Linux_fsck.png]]
```

```ad-example
title: OSX - First Aid
collapse:close
![[OSX_FistAid.png]]
```

### Defrag

```ad-example
title: Windows - Defrag CLI
collapse:close
![[Win_Defrag_CLI.png]]
```

```ad-example
title: Windows - Defrag App 
collapse:close
![[Win_Defrag_App.png]]]
```

```ad-example
title: OSX - Defrag App
collapse:close
![[OSX_Defrag_App.png]]
```

```ad-example
title: Linux - Defrag CLI
collapse:close
![[Linux_Defrag_CLI.png]]
```

# Objectives
---
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]