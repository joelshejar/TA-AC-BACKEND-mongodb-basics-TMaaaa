writeCode

Run these shell commands in mongo shell:

- db.version()//4.4.6

- db.stats()
{
	"db" : "test",
	"collections" : 0,
	"views" : 0,
	"objects" : 0,
	"avgObjSize" : 0,
	"dataSize" : 0,
	"storageSize" : 0,
	"totalSize" : 0,
	"indexes" : 0,
	"indexSize" : 0,
	"scaleFactor" : 1,
	"fileSize" : 0,
	"fsUsedSize" : 0,
	"fsTotalSize" : 0,
	"ok" : 1
}

- db.help()
DB methods:
	db.adminCommand(nameOrDocument) - switches to 'admin' db, and runs command [just calls db.runCommand(...)]
	db.aggregate([pipeline], {options}) - performs a collectionless aggregation on this database; returns a cursor
	db.auth(username, password)
	db.cloneDatabase(fromhost) - will only function with MongoDB 4.0 and below
	db.commandHelp(name) returns the help for the command
	db.copyDatabase(fromdb, todb, fromhost) - will only function with MongoDB 4.0 and below
	db.createCollection(name, {size: ..., capped: ..., max: ...})
	db.createUser(userDocument)
	db.createView(name, viewOn, [{$operator: {...}}, ...], {viewOptions})
	db.currentOp() displays currently executing operations in the db
	db.dropDatabase(writeConcern)
	db.dropUser(username)
	db.eval() - deprecated
	db.fsyncLock() flush data to disk and lock server for backups
	db.fsyncUnlock() unlocks server following a db.fsyncLock()
	db.getCollection(cname) same as db['cname'] or db.cname
	db.getCollectionInfos([filter]) - returns a list that contains the names and options of the db's collections
	db.getCollectionNames()
	db.getLastError() - just returns the err msg string
	db.getLastErrorObj() - return full status object
	db.getLogComponents()
	db.getMongo() get the server connection object
	db.getMongo().setSecondaryOk() allow queries on a replication secondary server
	db.getName()
	db.getProfilingLevel() - deprecated
	db.getProfilingStatus() - returns if profiling is on and slow threshold
	db.getReplicationInfo()
	db.getSiblingDB(name) get the db at the same server as this one
	db.getWriteConcern() - returns the write concern used for any operations on this db, inherited from server object if set
	db.hostInfo() get details about the server's host
	db.isMaster() check replica primary status
	db.hello() check replica primary status
	db.killOp(opid) kills the current operation in the db
	db.listCommands() lists all the db commands
	db.loadServerScripts() loads all the scripts in db.system.js
	db.logout()
	db.printCollectionStats()
	db.printReplicationInfo()
	db.printShardingStatus()
	db.printSecondaryReplicationInfo()
	db.resetError()
	db.runCommand(cmdObj) run a database command.  if cmdObj is a string, turns it into {cmdObj: 1}
	db.serverStatus()
	db.setLogLevel(level,<component>)
	db.setProfilingLevel(level,slowms) 0=off 1=slow 2=all
	db.setVerboseShell(flag) display extra information in shell output
	db.setWriteConcern(<write concern doc>) - sets the write concern for writes to the db
	db.shutdownServer()
	db.stats()
	db.unsetWriteConcern(<write concern doc>) - unsets the write concern for writes to the db
	db.version() current version of the server
	db.watch() - opens a change stream cursor for a database to report on all  changes to its non-system collections.




Write code to

- create a database of your country name. use India
- check list of databases to see newly created database. 
- check which database you are currently connected to ? India
