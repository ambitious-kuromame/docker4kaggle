# docker4kaggle
Dockerfiles for DeepLearningVM @ GCP


## Detail
This Docker file is for GCP DeepLearning VM.
I tested on the VM such as ...

```text
version :M21
OS      :Debian 9
CUDA    :CUDA10.0
```

## How to use

```bash
docker build ./ -t kaggle_base
mkdir project
docker run --runtime=nvidia -p 8888:8888 -d -v ~/project:/root/user/project --name test kaggle_base /sbin/init
```
