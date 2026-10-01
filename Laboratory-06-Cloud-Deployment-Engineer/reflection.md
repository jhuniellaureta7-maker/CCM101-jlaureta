# Mission Reflection

### 1. How does writing a docker-compose.yml file make a cloud engineer's job easier compared to manually
typing commands? 
Writing a docker-compose.yml file is much easier for a cloud engineer since the configuration of multiple containers can be described in one file. Instead of writing each container’s specific command, the Docker Compose will utilize the YAML file to compose an application of multiple containers which makes the process more organized and repeatable.

### 2. What happens if you make an indentation error (like using a Tab instead of Spaces) in a YAML file?
YAML indentation is very important because the structure of the file depends on it. If I use a Tab or an incorrect indentation, then Docker Compose may not be able to parse the file correctly and may give an error. This experience taught me that a minor formatting error is enough to make an infrastructure description work incorrectly.

### 3. Why did we use environment variables (like MYSQL_PASSWORD) in the Compose file? 
Environment variables such as `MYSQL_PASSWORD` serve to transfer information for configuring the operation of the containers. It is notable that in the laboratory, these variables have been used to configure the MariaDB database and for the Nextcloud application to connect to it. The `MYSQL_HOST=database` variable specifies the location of the service that will be used by the Nextcloud application.

### 4. How did it feel to deploy a fully functional enterprise cloud storage system (Nextcloud) in just a few minutes?
It was always interesting to set up a private cloud storage platform like Nextcloud in just several minutes using a utility like DockerCompose. Instead of spending a lot of time installing each necessary part for the cloud to work, I simply allowed DockerCompose to pull images and launch database and app services. This experience allowed me to understand how exactly the processes of cloud deployment may be automatized and thus made more effective.

### 5. How has your understanding of Cloud Computing evolved since Mission 1? 
Since mission 1, my understanding of Cloud Computing has evolved. I started with the basics of the cloud, then I learned about containers and object storage. Now I am at the level of multi-containers applications deployment. This laboratory allowed me to discover the Infrastructure as Code and to realize that it is possible to configure the cloud with configuration files.
