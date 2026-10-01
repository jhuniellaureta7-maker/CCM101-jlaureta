### Docker Compose Configuration

### 1. What does the `services:` block do?

The `services:` block defines the containers that will be created and managed by Docker Compose. In our YAML file, it contains the **database** (MariaDB) and **app** (Nextcloud) containers.

### 2. How did the Nextcloud app container know how to find the database container?

The Nextcloud app uses the `MYSQL_HOST=database` environment variable. The word `database` refers to the database service name in the `docker-compose.yml`, allowing Nextcloud to connect to the MariaDB container.

### 3. What is the difference between `docker run` and `docker-compose up -d`?

`docker run` is used to create and run a single container using command-line options. `docker-compose up -d` uses the `docker-compose.yml` file to create and run multiple related containers together with their configurations and connections.
