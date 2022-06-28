(1) Git clone the repository
```
git clone https://github.com/ZhiangChen/instance_segmentation_remote_sensing.git
```

(2) Build a docker image
```
docker build -t isrs .
```

(3) Run the docker image in a container
```
docker run -p 8888:8888 -it --name isrs -v host_dir:/root/isrs/ isrs
```

(4) Run jupyter notebook in the container
```
cd 
jupyter notebook --allow-root --ip=0.0.0.0
```

(5) Access to a new terminal in the container
```
docker exec -it isrs bash
```

