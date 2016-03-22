####Backups
* Backups are run as the sql service account 

####Recovery model
* Full to bulk logged does not break the chain

####Database
* you cannot delete the first file created in a db
* emptying file distributes the data accross the files in the same filegroup

####Restore
* suspect_pages are kept in msdb

####HA
* asynchronous mirroring enterprise only feature

####CPU
* trace flag 8649 - use to force parallelism by dropping cost theshold to 0. useful for development 

####Sleeping Process
* Sleeping process with high cpu and IO does not indicate current performance (entries are cumulative)

####INternals
* sys.sysallocunits - system table which identifies root_page and IAM page for option
