#####Disk layout
* tempdb/data/logs - seperate disks
* tempdb raid 10
* log raid 10
* data raid 5
* No difference with SAN as storage shared
* OBR10 - https://community.spiceworks.com/topic/262196-one-big-raid-10-the-new-standard-in-server-storage

#####Tempdb
* files 1:1 with CPU up to 8
* https://support.microsoft.com/en-us/kb/2154845

#####Data files to CPU
* .25:1 
* https://technet.microsoft.com/en-gb/library/cc966534.aspx
