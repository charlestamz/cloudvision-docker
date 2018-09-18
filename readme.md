本项目目的是建立 包含cuda 9.0 cudnn 7 opencv 3.4.2的c++编译环境

1. 安装nvidia-docker

ref https://github.com/NVIDIA/nvidia-docker

2. 获取docker镜像

```
sudo docker pull nvidia/cuda:9.0-cudnn7-devel-ubuntu16.04
sudo nvidia-docker run -it nvidia/cuda:9.0-cudnn7-devel-ubuntu16.04
```

3. build docker
```
docker build -t cloudvision .
```

4. 运行docker

```
sudo nvidia-docker run -it cloudvision:latest
```