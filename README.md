# Udemy Docker & Kubernetes course assignment problem

## Commands

### Python app

Building image

```
docker build . -t python-image
```

Running container

```
docker run -it --name python-app python-image
```

Stop container 

```
docker stop python-app
```

Restart container

```
docker start -i -a python-app
```

Remove container

```
docker rm python-app
```

Remove image

```
docker rmi python-image
```

Build image with tag

```
docker build -t bmi-app:1 .
```

Run container with 

```
docker run -it --name bmi-app --rm bmi-app:1
```

### Node app

Building image

```
docker build . -t node-image
```

Running container

```
docker run -p 3000:3000 --name node-app node-image
```

Stop container

```
docker stop node-app
```

Restart container

```
docker start node-app
```

Remove container

```
docker rm python-app
```

Remove image

```
docker rmi node-image
```

Build image with tag

```
docker build -t node-demo:latest .
```

Run container with auto remove after container stop

```
docker run -p 8000:3000 -d --name node-app --rm node-demo:latest
```

### Generic

Remove all untagged images

```
docker image prune
```

Remove all images including tagged ones

```
docker image prune -a
```

Rename the name and tag of image.
Renaming does not delete the original but it creates a clone with the new name. 

```
docker tag node-demo:latest harukaichinose/node-hello-world
```

Login to docker 

```
docker login
```

Push Docker image to Docker Hub

```
docker push harukaichinose/node-hello-world
```