
---
type: note-type/braindump
tags: [system-engineering]
---

# Howto

## Disk management

Create and management partitions

[How to create a Recovery Partition in Microsoft Windows 10/11](https://www.youtube.com/watch?v=hlNtLcFqfOo)

Commands

Example: How to create a recovery partition
```
diskpart
DISKPART> list disk
DISKPART> select disk (DiskNumber from list disk)
DISKPART> list partition
DISKPART> select partition (Partitions Number from Drive c:)
DISKPART> shrink desired=700
DISKPART> create partition primary
DISKPART> format quick fs=ntfs label="winRE"
DISKPART> set id=de94bba4-06d1-4d40-a16a-bfd50179d6ac
DISKPART> exit
C:\WINDOWS\system32> reagentc /enable
REAGENTC.EXE: Operation Successful
```

Example2: How to delete a partition

1.  At a command prompt, type diskpart.
2.  At the DISKPART prompt, type select disk 0 (Selects the disk.)
3.  At the DISKPART prompt, type list partition.
4.  At the DISKPART prompt, type select partition 4 (Selects the partition.)
5.  At the DISKPART prompt, type delete partition override
6.  At the DISKPART prompt, type exit.

Microsoft Build
[Get-Disk](https://learn.microsoft.com/en-us/powershell/module/storage/get-disk?view=windowsserver2022-ps)

