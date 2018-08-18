# dse-docker-project-template
Quickstart project template to start DataStax Enterprise and Studio in Docker

## Contents
This simple project contains:

* A docker-compose file that will start:
  * a single instance of DataStax Enterprise
  * a single instance of DataStax Studio that will connect to DSE
* Stubbed out "data" and "notebooks" directories 
  * The DSE image mounts the "data" directory as its file storage location
  * The Studio image mounts the "notebooks" directory as its notebook storage location

This project is a quick way to get a simple DSE environment running on your local machine, which is very useful for testing purposes.

The project represents an opinionated viewpoint, in that data storage is externalized from the containers, allowing you to preserve data even if you have to recreate a container.
