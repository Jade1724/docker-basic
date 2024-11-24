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

### Generic

Remove all untagged images

```
docker image prune
```

Remove all images including tagged ones

```
docker image prune -a
```
