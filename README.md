win64-xdark-5.3
##master branch##
===============

wim images for xDark Deluxe 5.3

---------------

I, alp1ne do not condone illegal activation in any way, shape, or form.
I am not responsible for broken features and/or core utilities.
I am also NOT at fault if your computer does not act in a desirable manner as a result of this operationg system.

--------------

**Installation Instructions -**

• Find an 8 gb or larger USB flash drive.

• Open diskpart "windows+R diskpart ENTER"

• Type in LIST DISK, and find your USB and note it's number.
	
	Microsoft DiskPart version 6.1.7601
	On computer: YOUR-PC-NAME
	
	DISKPART> list disk

  	Disk ###  Status         Size     Free     Dyn  Gpt

  	Disk 0    Online          931 GB  1024 KB
  	Disk 1    Online           59 GB  2860 MB
  	Disk 2    Online         8549 MB      0 B

	DISKPART>
	
• Type SELECT DISK X, where X is the number of your USB drive.

	DISKPART> select disk X
	
	Disk X is now the selected disk.

• Type CLEAN
	DISKPART> clean

	DiskPart succeeded in cleaning the disk.
	
• Type CREATE PARTITION PRIMARY
	DISKPART> create partition primary

	DiskPart succeeded in creating the specified partition.

• Type SELECT PARTITION 1

• Type FORMAT FS=NTFS QUICK

	DISKPART> format fs=ntfs quick

  100 percent completed

	DiskPart successfully formatted the volume.
	
• Type ACTIVE

	DISKPART> active

	DiskPart marked the current partition as active.

• If you have a WINDOWS 7 x64 installation .iso, unzip it. If you have a CD, copy it to the flash drive.

• Copy the files to the drive.

• Boot and install.
