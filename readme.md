## Preconditions

### postgres
psql and pg_dump command must be visible from commmand line

### properties
copy default.properties to local.properties

change settings für db,user and password 

## dump DB
    mvn compile -Pdump-db -Dfile=dump.sql
    
## drop, create and restore DB
    mvn compile -Pdrop-create-and-restore -Dfile=dump.sql
    
