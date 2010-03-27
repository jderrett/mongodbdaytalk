!SLIDE bullets incremental transition=blindY
# Why MongoDB is awesome
* It's easy to install

!SLIDE commandline incremental
## Get it

	$ curl -O http://downloads.mongodb.org/osx/mongodb-osx-x86_64-1.4.0.tgz
	$ gunzip mongodb-osx-x86_64-1.4.0.tgz
	$ cd mongodb-osx-x86_64-1.4.0/bin
	$ ./mongod
	
	./mongod --help for help and startup options
	Fri Mar 26 23:41:55 Mongo DB : starting : pid = 51942 port = 27017 dbpath = /data/db/ master = 0 slave = 0  64-bit 
	Fri Mar 26 23:41:55 db version v1.4.0, pdfile version 4.5
	Fri Mar 26 23:41:55 git version: 514f8bbab657c1dc110d45eea6ea33de296dbb26
	Fri Mar 26 23:41:55 sys info: Darwin erh2.10gen.cc 9.6.0 Darwin Kernel Version 9.6.0: Mon Nov 24 17:37:00 PST 2008; root:xnu-1228.9.59~1/RELEASE_I386 i386 BOOST_LIB_VERSION=1_37
	Fri Mar 26 23:41:55 waiting for connections on port 27017
	Fri Mar 26 23:41:55 web admin interface listening on port 28017

!SLIDE bullets
# Why MongoDB is awesome
* It's easy to install
* It runs on everything
* It connects with everything
* Lots of devs involved (that's us!)
* It's friggin' PRODUCTIVE

!SLIDE bullets incremental transition=blindY
# Other reasons

* It can act like a document database (i.e. structure is arbitrary)
* It can act like a relational database (i.e. "child" objects or MongoMapper Embedded Doc)
* You can query it all sorts of ways (like regexes!)

!SLIDE bullets incremental transition=blindY
# Other other reasons

* Databases on the fly!
* Collections on the fly!
* Queries on the fly (i.e. no predefined "views")!
* It replicates!

