!SLIDE
# Replication Setup
## Bring up master server
## Bring up N slave servers
## Replicate

!SLIDE commandline
# Replication
## Server 1 - master
	$ mongod --master
## Server 2 - slave
	$ mongod --slave --source <masterhostname>[:<port>]
## Server 3 - slave
	$ mongod --slave --source <masterhostname>[:<port>]
## ...
## Server N