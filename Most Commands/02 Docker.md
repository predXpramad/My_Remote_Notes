Docker (Basic -> Advance)

**Docker Commands Reference Table**
| Command              | Syntax             | Usage (Brief Explanation)                    |
| -------------------- | ------------------ | -------------------------------------------- |
| Check Docker Version | `docker --version` | Shows the installed Docker version.          |
| Docker System Info   | `docker info`      | Displays detailed Docker system information. |
| Help for Commands    | `docker --help`    | Lists all Docker commands.                   |

---
---

**Image Management Commands**
| Command                | Syntax                              | Usage                               |
| ---------------------- | ----------------------------------- | ----------------------------------- |
| Search Image           | `docker search image_name`          | Searches Docker Hub for images.     |
| Pull Image             | `docker pull image_name`            | Downloads an image from Docker Hub. |
| List Images            | `docker images`                     | Displays all downloaded images.     |
| Remove Image           | `docker rmi image_id`               | Deletes a Docker image.             |
| Remove Multiple Images | `docker rmi image1 image2`          | Deletes multiple images.            |
| Build Image            | `docker build -t image_name .`      | Builds an image from a Dockerfile.  |
| Tag Image              | `docker tag image_id repo:tag`      | Assigns a tag to an image.          |
| Push Image             | `docker push repo/image_name`       | Uploads an image to Docker Hub.     |
| Save Image             | `docker save image_name > file.tar` | Saves image to a tar file.          |
| Load Image             | `docker load < file.tar`            | Loads image from tar file.          |
| Image History          | `docker history image_name`         | Shows layers used in the image.     |
| Inspect Image          | `docker inspect image_name`         | Displays detailed image metadata.   |

---
---

**Container Management Commands**
| Command                   | Syntax                                        | Usage                                        |
| ------------------------- | --------------------------------------------- | -------------------------------------------- |
| Run Container             | `docker run image_name`                       | Creates and runs a container.                |
| Run Interactive Container | `docker run -it image_name`                   | Runs container with interactive terminal.    |
| Run Container with Name   | `docker run --name container_name image_name` | Assigns name to container.                   |
| Run in Background         | `docker run -d image_name`                    | Runs container in detached mode.             |
| List Running Containers   | `docker ps`                                   | Shows currently running containers.          |
| List All Containers       | `docker ps -a`                                | Shows all containers including stopped ones. |
| Start Container           | `docker start container_id`                   | Starts a stopped container.                  |
| Stop Container            | `docker stop container_id`                    | Stops a running container.                   |
| Restart Container         | `docker restart container_id`                 | Restarts a container.                        |
| Pause Container           | `docker pause container_id`                   | Temporarily pauses a container.              |
| Unpause Container         | `docker unpause container_id`                 | Resumes paused container.                    |
| Remove Container          | `docker rm container_id`                      | Deletes a stopped container.                 |
| Remove Running Container  | `docker rm -f container_id`                   | Force removes running container.             |
| Rename Container          | `docker rename old_name new_name`             | Renames a container.                         |

---
---

**Container Interaction Commands**
| Command             | Syntax                                    | Usage                                   |
| ------------------- | ----------------------------------------- | --------------------------------------- |
| Execute Command     | `docker exec container_id command`        | Runs command inside container.          |
| Interactive Shell   | `docker exec -it container_id bash`       | Opens terminal inside container.        |
| View Logs           | `docker logs container_id`                | Shows container logs.                   |
| Follow Logs         | `docker logs -f container_id`             | Streams container logs in real time.    |
| Copy Files          | `docker cp source container_id:path`      | Copies files to container.              |
| Copy From Container | `docker cp container_id:path destination` | Copies files from container.            |
| Attach Container    | `docker attach container_id`              | Connects terminal to running container. |
| Container Stats     | `docker stats`                            | Shows resource usage of containers.     |
| Inspect Container   | `docker inspect container_id`             | Displays detailed container info.       |
| Top Processes       | `docker top container_id`                 | Shows processes running in container.   |

---
---

**Volume Management Commands**
| Command               | Syntax                                  | Usage                       |
| --------------------- | --------------------------------------- | --------------------------- |
| Create Volume         | `docker volume create volume_name`      | Creates a Docker volume.    |
| List Volumes          | `docker volume ls`                      | Lists all volumes.          |
| Inspect Volume        | `docker volume inspect volume_name`     | Shows volume details.       |
| Remove Volume         | `docker volume rm volume_name`          | Deletes a volume.           |
| Remove Unused Volumes | `docker volume prune`                   | Removes unused volumes.     |
| Mount Volume          | `docker run -v volume_name:/path image` | Mounts volume to container. |

---
---

**Network Management Commands**
| Command                | Syntax                                        | Usage                               |
| ---------------------- | --------------------------------------------- | ----------------------------------- |
| List Networks          | `docker network ls`                           | Shows available networks.           |
| Create Network         | `docker network create network_name`          | Creates a new network.              |
| Inspect Network        | `docker network inspect network_name`         | Shows network configuration.        |
| Connect Container      | `docker network connect network container`    | Connects container to network.      |
| Disconnect Container   | `docker network disconnect network container` | Disconnects container from network. |
| Remove Network         | `docker network rm network_name`              | Deletes a network.                  |
| Remove Unused Networks | `docker network prune`                        | Removes unused networks.            |

---
---

**Docker System & Maintenance Commands**
| Command                   | Syntax                   | Usage                                |
| ------------------------- | ------------------------ | ------------------------------------ |
| Disk Usage                | `docker system df`       | Shows disk usage by Docker.          |
| Remove Stopped Containers | `docker container prune` | Deletes all stopped containers.      |
| Remove Unused Images      | `docker image prune`     | Deletes unused images.               |
| Remove Everything Unused  | `docker system prune`    | Cleans containers, images, networks. |
| Aggressive Cleanup        | `docker system prune -a` | Removes all unused data.             |

---
---

**Docker Compose Commands**
| Command           | Syntax                 | Usage                             |
| ----------------- | ---------------------- | --------------------------------- |
| Start Services    | `docker compose up`    | Creates and starts containers.    |
| Run in Background | `docker compose up -d` | Runs services in detached mode.   |
| Stop Services     | `docker compose down`  | Stops and removes containers.     |
| Build Services    | `docker compose build` | Builds services from Dockerfile.  |
| View Logs         | `docker compose logs`  | Shows service logs.               |
| List Services     | `docker compose ps`    | Shows running compose containers. |

---
---

**Advanced Docker Commands**
| Command                 | Syntax                                  | Usage                                |
| ----------------------- | --------------------------------------- | ------------------------------------ |
| Login to Docker Hub     | `docker login`                          | Authenticates with Docker Hub.       |
| Logout                  | `docker logout`                         | Logs out from Docker Hub.            |
| Docker Events           | `docker events`                         | Shows real-time Docker events.       |
| Export Container        | `docker export container_id > file.tar` | Exports container filesystem.        |
| Import Image            | `docker import file.tar image_name`     | Creates image from tar file.         |
| Commit Container        | `docker commit container_id image_name` | Saves container as new image.        |
| Build Multi-stage Image | `docker build --target stage`           | Builds specific stage in Dockerfile. |
| Check Processes         | `docker top container_id`               | Displays container processes.        |

---
---

Most Frequently Used Docker Commands (Top 10)
1. docker pull image
2. docker run -it image
3. docker ps
4. docker images
5. docker stop container
6. docker rm container
7. docker rmi image
8. docker build -t image .
9. docker exec -it container bash
10. docker compose up -d