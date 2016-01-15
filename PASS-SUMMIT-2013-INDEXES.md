## Indexes half day session Gail Shaw
* B-tree = balanced tree
* data pages, leaf level of clustered index
* seek=looking down the b-tree
* scan =going through all leaf pages
* SQL can read forward and backwards along the  level
* DBCC IND(db_name,table_name,index_id) - pages to object *Enable dbcc traceon(3604)*
* DBCC IND page type 10=IAM,2=index,1=data
* DBCC PAGE(db_name,file_id,page_num,display method) - raw output of page *Enable dbcc traceon(3604)*
* DBCC PAGE can be used to find object *deadlock/locking chain*
* clustered index always 1
* leaf level is level 0
* root is always in system tables, old sysindexes has root column
