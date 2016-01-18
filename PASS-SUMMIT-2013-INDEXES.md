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
* Clus index contains the table/b-tree on top/uniquefier added to non-cluster column
* 2 thougts 1) clustered index on most frequently used column 2) clustered index to organise colmns
* page splits occur upwards also/new root created
* page splits/sec measures new allocations/new extended event to meahure this in 2012
* heap has a RID = file,page,slot array
* if unique is defined the cluster key is at leaf only/if not unique then key is at ever level
* IX should return less than 1% of rows in table or covering
* dont depend on implicit behaviour - dont add cidx to idx unless you have to 
* multiple equality queries searched simultaneous (order does not matter) *test*
* index limit 900bytes, 16 columns
* gail shaw - simple talk, perfomance tuning strategy
* dont put most selective column by default/covering over selectivity
* equality first, inequality second.*test*
* OR operation requires index on each columns
* case = function= no index
* joins=where columns first, then join columns

##Indexes - Tim Chapman
* heap 
  * unorder   
  * table withou clustered index
  * PFS page used to check for pages with space (64 mb allocation)
  * ALTER TABLE REBUILD to reduce fragmentation , forwarding pointers
* 
