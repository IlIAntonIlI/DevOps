# DevOps

[DockerHub repository](https://hub.docker.com/repository/registry-1.docker.io/iliantonili/docker-practice/)

## Steps: 
- ###  First step (build the image):

```
docker build . -t docker-app
```

 - ### Second step (check all available images and their ids):

```
docker images
```

- ### Third step (run the container with limits):

In current example limits:
1) 2GB of memory
2) 1.5 CPUS

Run the container with memory(`2GB`) and CPU limits(`1.5 CPU`) on `80` port:

```
docker run -m="2g" --cpus="1.5" --rm --name docker-app -p 80:80 -d docker-app
```