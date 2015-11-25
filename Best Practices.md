#####Disk layout
* tempdb/data/logs - seperate disks
* tempdb raid 10
* log raid 10
* data raid 5
* No difference with SAN as storage shared
* OBR10 - https://community.spiceworks.com/topic/262196-one-big-raid-10-the-new-standard-in-server-storage
* Example sizes - http://www.sqltuners.net/blog/13-05-16/SQL_Tuners_Disk_Partition_Best_Practices.aspx

#####Tempdb
* files 1:1 with CPU up to 8
* https://support.microsoft.com/en-us/kb/2154845

#####Data files to CPU
* .25:1 
* https://technet.microsoft.com/en-gb/library/cc966534.aspx
* http://sqlblog.com/blogs/linchi_shea/archive/2007/01/29/how-many-data-files-should-i-create-for-a-user-database.aspx
* http://www.sqlskills.com/blogs/paul/benchmarking-do-multiple-data-files-make-a-difference/

#####Memory for OS
* https://sqlserverperformance.wordpress.com/2009/10/29/suggested-max-memory-settings-for-sql-server-20052008/
