# docker-kubernetes-foundation

The course contains the following parts.
- Docker, Container
- Docker Registry
- Kubernetes

Initial setup required:
- VS Code
- Docker Desktop with Kubernetes enabled
- Dockerhub account

## Container
- Container is a single unit of deployment.
## Docker
- It is a container runtime.
- Uses a Dockerfile to create image.

```Dockerfile
FROM node:20-alpine # BASE IMAGE for the application
WORKDIR /app # This is the directory of the container from where commands are run
COPY . . # Copy files from local to container
RUN yarn install --production # Install dependencies for the app
CMD ["node", "./src/index.js"] # The command to run when the container starts
EXPOSE 3000 # The port of the container which is exposed for communication
```
