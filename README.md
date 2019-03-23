# docker4kaggle
Dockerfiles for DeepLearningVM @ GCP

## How to use

```bash
docker build ./ -t kaggle_base
mkdir project
docker run --runtime=nvidia -p 8888:8888 -d -v ~/project:/root/user/project --name test kaggle_base /sbin/init
```
