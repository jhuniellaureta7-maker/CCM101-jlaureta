# Mission Reflection

## 1. Docker Container vs Virtual Machine Setup

A Docker container can be deployed much faster than installing an operating system on a Virtual Machine. A VM normally requires a complete guest operating system, which takes more time and resources to start. With Docker, an existing image can be pulled and used to create a container within a short amount of time. This makes containers useful for workloads that require fast and repeatable deployment.

## 2. Importance of Port Mapping

Port mapping such as `-p 8080:80` is necessary because it connects a port on the host machine to a port inside the container. In this activity, port 8080 on the host was mapped to port 80 where Nginx was running inside the container. This allowed me to access the Nginx web server using `http://localhost:8080`.

## 3. What Happens When docker rm Is Used?

The `docker rm` command removes a stopped container from the Docker environment. The container itself is deleted, so its writable container layer and information associated with that container are no longer available. Data that needs to survive container removal should be stored using persistent storage such as volumes.

## 4. Containerization and DevOps

Containerization can improve collaboration between software developers and IT operations teams because applications can be packaged with their dependencies in a consistent environment. Developers can create and test containers while operations teams can deploy the same container image. This supports repeatable deployments and can reduce differences between development and production environments.

## 5. GitHub Portfolio Evolution

My GitHub portfolio is becoming more organized as I complete each cloud computing laboratory activity. In this laboratory, I added documentation about Virtual Machines, containers, Docker commands, Nginx deployment, and container lifecycle management. The screenshots also provide evidence of the technical tasks I completed. This laboratory helped me improve both my cloud computing knowledge and my ability to document technical work.
