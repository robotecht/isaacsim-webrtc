# isaacsim-webrtc
Demo showing Isaac Sim hosted using the web client.

# Isaac Sim Container Installation

Perform the container installation of Isaac Sim following the [official documentation](https://docs.isaacsim.omniverse.nvidia.com/latest/installation/install_container.html).


```bash

mkdir isaac-sim-docker

cd isaac-sim-docker/

touch Dockerfile

nano Dockerfile

```

Add these contents into the docker file

```bash
ROM nvcr.io/nvidia/isaac-sim:4.5.0

RUN apt-get update && apt-get -y upgrade
```
Build docker file

```bash

docker build -t isaacsim:nr . 

```
