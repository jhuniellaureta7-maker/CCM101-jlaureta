## Mission Overview
In this laboratory activity, I monitored the Linux host, deployed an Nginx web server using Docker, generated HTTP requests, analyzed application logs, and checked container resource metrics.

## Objectives
- Monitor host RAM and disk capacity.
- Observe running processes and CPU load.
- Deploy an Nginx container.
- Generate successful and failed HTTP requests.
- Analyze Docker logs and real-time container metrics.
- Document the results using Markdown.

## Monitoring Commands Executed
```bash
free -h
df -h /
top
docker run -d -p 8080:80 --name client-website nginx
docker ps
curl -i http://localhost:8080/
curl -i http://localhost:8080/hidden-admin-page
docker logs client-website
docker stats
```

## Skills Learned
I managed to learn how to monitor Linux system resources, deploy a containerized web server, make HTTP requests to it, troubleshoot errors using the application’s logs, and monitor CPU and memory usage with Docker.
