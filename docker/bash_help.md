1. Build a docker image
```
docker build -t isrs .
```

2. Run the docker image in a container
```
docker run -p 8888:8888 -it --name isrs isrs
```

3. Run jupyter notebook in the container
```
cd 
jupyter notebook --allow-root --ip=0.0.0.0
```

4. Access to a new terminal in the container
```
docker exec -it isrs bash
```

5. Mount volume
```
docker run -p 8888:8888 -it --name isrs -v host_dir:container_dir isrs
```
