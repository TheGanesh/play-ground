# play-ground
Central project for all future POCs

### Docker Compose
Docker compose is used to download and run the 3rd party applications.  Note: All docker compose commands must be run from the folder containing the docker-compose.yml file.
#### Start Applications
* `docker-compose up -d` <br/>
#### Shutdown Applications
* `docker-compose down`
#### Cassandra Commands
The following are commonly used cassandra commands
#### To connect to Cassandra command line
* `docker exec -it my_cassandra_1 cqlsh`
#### Cassandra Database Setup
Execute cql scripts in `./play-ground/src/main/resources/schema.cql` sequentially, this is a one time activity.  
#### To Connect to container
Typically done for debugging purposes
* `docker exec -it my_cassandra_1 bash` 
* `docker exec -it my_cassandra_1 nodetool status`
   
## Running in local
```
mvn clean install spring-boot:run
```

