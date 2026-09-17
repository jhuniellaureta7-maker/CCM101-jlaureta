# Laboratory 04 – Cloud-Native Engineer

**Student Name:** Jhuniel Laureta
**Subject:** CCM101 – Cloud Computing

## Mission Overview

This laboratory activity focuses on cloud-native technologies, particularly containers and Docker. The activity compares traditional Virtual Machines with containers and demonstrates how Docker can be used to deploy and manage an Nginx web server.

## Objectives

* Differentiate between Virtual Machines and containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull, run, manage, and terminate an Nginx container.
* Document container operations using Markdown.
* Continue developing a structured GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
docker info
```

### Nginx Deployment

```bash
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

This lab helped me understand the core differences between VMs and containers, not just in theory but hands-on. I got to verify that Docker was installed and working, pull an image, and run an Nginx container from it. Along the way I picked up how port mapping works, how to actually test that a web server is running through curl, and how to manage a container's lifecycle using different Docker commands.

## Challenges Encountered

The trickiest part for me was getting a solid grasp of the Docker commands, especially figuring out how the host port and container port relate to each other. I also had to double-check that the Nginx container was actually up and running before I tried testing it with curl - otherwise the test wouldn't make sense. On top of that, keeping the screenshots and Markdown documentation organized took more effort than I expected, since everything needed to line up properly with each step.
