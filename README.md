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
