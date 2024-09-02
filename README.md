# Gcloud Docker Container
Initial code for using Google's gcloud APIs from a docker container, instructions to use below.


## Gcloud
Adapted from documentation: https://cloud.google.com/sdk/docs/downloads-docker

1. Clone this repo

2. Build docker container

```bash
cd gcloud
docker compose build gcloud
```
3. Auth Google

```bash
docker run -ti --name gcloud-config gcloud-gcloud gcloud auth login
```

4. Run docker container

```bash
docker-compose run gcloud /bin/bash
```

Now should have a terminal that can run gcloud commands from docker.
