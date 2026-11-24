# Laboratory 04: The Cloud-Native Engineer

## Mission Overview
CloudNova Technologies has a client whose traditional Virtual Machines boot slowly and waste RAM. In this mission, I compared VMs and containers, then used a KillerCoda Docker environment to deploy a containerized Nginx web server and document the exact commands so the client's IT team can replicate it.

## Objectives
- Differentiate between traditional Virtual Machines and Containers
- Access a Docker-enabled cloud environment using KillerCoda
- Execute fundamental Docker CLI commands
- Pull, run, manage, and terminate a containerized application (Nginx)
- Create professional technical documentation using Markdown
- Continue developing my GitHub Cloud Computing Portfolio

## Docker Commands Executed

**Checkpoint 3**
```bash
docker --version
docker ps
```

**Checkpoint 4**
```bash
docker pull nginx
docker run -d --name my-nginx -p 8080:80 nginx
curl http://localhost:8080
```

**Checkpoint 5**
```bash
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx
docker ps -a
```

## Skills Learned
- Explaining the architectural differences between VMs and containers
- Verifying that Docker is installed and running on Linux
- Pulling images and running containers in detached mode
- Exposing a container port to the host using port mapping
- Managing the container lifecycle (run, stop, remove)
- Documenting technical procedures in Markdown and organizing a GitHub repository

## Challenges Encountered
- Remembering the correct order of the port mapping format (`host:container`, so `8080:80`)
- Understanding the difference between `docker ps` and `docker ps -a` when checking stopped containers
- Capturing clear screenshots from the KillerCoda terminal and uploading them to the correct folder in GitHub

## Files
- [virtualization-vs-containers.md](virtualization-vs-containers.md)
- [docker-deployment.md](docker-deployment.md)
- [reflection.md](reflection.md)
- `screenshots/`
