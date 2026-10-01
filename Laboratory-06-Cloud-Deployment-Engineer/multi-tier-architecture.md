## What is Two-Tier Architecture?

The two-tier application architecture is considered as an application structure where the software is divided into two different layers, Web/Application Tier and Database Tier based on similar functionalities. These two units work in coordination to provide an effective application service.

## The Web/Application Tier

The Web/Application Tier is responsible for providing the user interface and handling HTTP requests from users. In this laboratory, the Nextcloud container serves as the web/application tier.

## The Database Tier

On the other hand, the database tier is responsible for storing all the persistent data of the application, including the user accounts of the system. In this experiment, the database is managed by using the MariaDB container.

## Why Separate Them?

The purpose of separating the web application and database is to make the system organized and efficient. Both the web container and database container serve different purposes and functionalities. Thus, combining these two services in a single container is not recommended.

Moreover, this process will make the application easily scalable and manageable compared to a combined application system. Using Docker Compose to define the application’s services makes the two-tier structure more organized and manageable. This tool helps to let these two services communicate while maintaining their isolation in terms of functionality.
