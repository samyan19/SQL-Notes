####Multiple Files
* you *cannot* empty the first database file (dbcc shrinkfile (file, emptyfile))
* data from emptyfile is distributed evenly accross the remaining files
