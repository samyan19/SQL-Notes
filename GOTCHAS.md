####Recovery model
* Full to bulk logged does not break the chain

####Database
* you cannot delete the first file created in a db
* emptying file distributes the data accross the files in the same filegroup

####Restore
* suspect_pages are kept in msdb

####HA
* asynchronous mirroring enterprise only feature