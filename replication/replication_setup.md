!SLIDE
# Replication Setup
## Bring up master server
## Bring up N slave servers
## Replicate

!SLIDE commandline incremental
# Launch master/slave(s)
## Server 1 - master
	$ mongod --master
## Server 2 - slave
	$ mongod --slave --source <masterhostname>[:<port>]
## Server 3 - slave
	$ mongod --slave --source <masterhostname>[:<port>]
## ...
## Server N

!SLIDE commandline
# Query for Source
	$ use local;
	$ db.sources.find();
	{ "_id" : ObjectId("4bacaf9d040f3de0474c2b9c"), 
	"host" : "10.179.46.140", 
	"source" : "main", "syncedTo" : { "t" : 1269720139000, "i" : 1 }, "localLogTs" : { "t" : 0, "i" : 0 } }


!SLIDE bullets incremental
# Slicehost master/slave setup
* Launch slice, install mongo, etc
* Clone slice(s)
* Start mongo on master
* Start mongo in slave mode for each slice