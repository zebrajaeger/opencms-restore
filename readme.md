## Preconditions

### postgres
psql and pg_dump command must be visible from commmand line

### properties
copy default.properties to local.properties

change settings für db,user and password 

## backup OpenCMS
 (dump DB, copy config files)
    mvn compile -Pbackup 
    
## restore OpenCMS 
(drop, create and restore DB, copy config files)
    mvn compile -Prestore
## remove dump data
    mvn compile -Pdelete
    
## handle multible dumps
change  'dump.id' in local.config or add -Ddump.id=... to commandline
    
