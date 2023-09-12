Docker is a powerful tool for containerization and managing containerized applications. Here are some useful Docker commands to help you work with containers:

1. **Basic Docker Commands**:
   - `docker pull <image_name>`: Downloads a Docker image from a registry.
   - `docker images`: Lists all locally available Docker images.
   - `docker ps`: Lists running containers.
   - `docker ps -a`: Lists all containers (both running and stopped).
   - `docker start <container_id>`: Starts a stopped container.
   - `docker stop <container_id>`: Stops a running container.
   - `docker restart <container_id>`: Restarts a container.
   - `docker rm <container_id>`: Removes a stopped container.
   - `docker rmi <image_id>`: Removes a Docker image.
   
2. **Creating and Running Containers**:
   - `docker run <image_name>`: Creates and starts a new container from an image.
   - `docker run -it <image_name> <command>`: Runs a container interactively with a specific command.
   - `docker run -d <image_name>`: Runs a container in detached mode (in the background).
   - `docker exec -it <container_id> <command>`: Executes a command inside a running container.
   
3. **Managing Images**:
   - `docker build -t <image_name> <path_to_Dockerfile>`: Builds a Docker image from a Dockerfile.
   - `docker push <image_name>`: Pushes a local image to a Docker registry.
   - `docker pull <image_name>`: Downloads an image from a Docker registry.
   - `docker tag <source_image> <target_image>`: Tags an image with a new name.

4. **Viewing Container Logs**:
   - `docker logs <container_id>`: Displays logs of a running container.

5. **Networking**:
   - `docker network ls`: Lists Docker networks.
   - `docker network create <network_name>`: Creates a custom Docker network.
   - `docker network connect <network_name> <container_name>`: Connects a container to a network.
   
6. **Volume Management**:
   - `docker volume create <volume_name>`: Creates a Docker volume.
   - `docker volume ls`: Lists Docker volumes.
   - `docker volume rm <volume_name>`: Removes a Docker volume.

7. **Inspecting Containers**:
   - `docker inspect <container_id>`: Displays detailed information about a container.
   - `docker inspect <image_name>`: Displays information about an image.

8. **Stopping and Removing Containers**:
   - `docker stop <container_id>`: Stops a running container.
   - `docker rm <container_id>`: Removes a stopped container.

9. **Docker Compose (for Multi-Container Applications)**:
   - `docker-compose up`: Starts services defined in a `docker-compose.yml` file.
   - `docker-compose down`: Stops and removes containers defined in a `docker-compose.yml` file.
   - `docker-compose logs`: Displays logs for services defined in a `docker-compose.yml` file.

These are some of the most commonly used Docker commands. Docker offers many more commands and options, so you can refer to the official Docker documentation for more detailed information and advanced usage.
