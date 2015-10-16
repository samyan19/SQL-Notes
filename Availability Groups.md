##Availabity Groups Notes - SQL in the City

* sys.dm_os_wait_stats
* execution plans can be different on the secondary, statistics, server settings
* primary sending, secondary receiving
* transaction delay on synchronous is both, async primary only
* alwaysOn_health session, hadr_database_flow_control_action, debug (extended events)
* 2008 r2 deadlocks captured in system health extended events
* some hadr_evnts are in the debug extended events channel
* AlwaysOn Health extended events trace
* 3 biggies - primary failover, readable secondaries fail, alwayson health
