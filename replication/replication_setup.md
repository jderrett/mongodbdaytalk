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

!SLIDE bullets incremental
# Slicehost master/slave setup
* Launch slice, install mongo, etc
* Clone slice(s)
* Start mongo on master
* Start mongo in slave mode for each slice
