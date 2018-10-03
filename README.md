# mongodb-docker-template
A docker-compose template repository for setting up a mongoDB instance with docker-networking.

# Use
* Clone the repo into a new folder
* within the repo folder run the command: `docker-compose up --build`

# Volumes
The 2 volumes created will use local folder locations within the repo/project directory to store the data writtent to the mongoDB instance.

# Networking
The container is setup to join a docker network called datanet. Any other containers which join this docker network can refer to this container (and access the mysql instance running within it) by using the hostname: `data-mongodb` and port `3306`
