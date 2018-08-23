# dse-docker-project-template
Quickstart project template to start DataStax Enterprise and Studio in Docker

## Contents
This simple project contains:

* A docker-compose file that will start:
  * A single instance of DataStax Enterprise with Search enabled
  * A single instance of DataStax Studio that will connect to DSE
* An additional, optional compose file: docker-compose-with-graph.yaml 
  * This configuration is the same as above except DSE is started with both Search and Graph enabled
  * This configuration works around some networking bugs/shortcomings of Docker compose and the Gremlin Server that prevent Studio from connecting to the Gremlin Server to run Gremlin queries
* Stubbed out "data" and "notebooks" directories 
  * The DSE image mounts the "data" directory as its file storage location
  * The Studio image mounts the "notebooks" directory as its notebook storage location

This project is a quick way to get a simple DSE environment running on your local machine, which is very useful for testing purposes.

