## Mission Overview

Laboratory 06 focuses on multi-tier application deployment using Docker Compose. Instead of deploying containers individually, a Nextcloud web application and a MariaDB database were defined in a YAML configuration file and deployed together as a multi-container stack.

## Objectives

* Explain the concept of multi-tier application architecture.
* Understand the purpose and structure of a `docker-compose.yml` file.
* Use the Linux command-line text editor Nano to create configuration files.
* Deploy a multi-container application using Docker Compose.
* Document Infrastructure as Code principles using Markdown.
* Continue developing the GitHub Cloud Computing Portfolio.

## Commands Executed

```bash
docker --version
docker ps
docker-compose --version
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

I learned how to create a Docker Compose YAML specification and utilize it to run various applications. I also learned how the Nextcloud image communicates with the MariaDB database container using the service name and environment variables. This learning opportunity allowed me to expand my knowledge of the said technologies and gain more experience with the Infrastructure as Code concept and Linux command line.
