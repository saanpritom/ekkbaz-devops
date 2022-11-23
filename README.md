# Container Orchester

This is a skeleton project. Here the directory defines various types of services. And the whole
project is configured to perform docker deployment for the [JWT-AUTH](https://github.com/saanpritom/ekkbaz-jwt-auth) and for the [BUSINESS-APP](https://github.com/saanpritom/ekkbaz-data-app).


## Requirements:

- Docker
- Docker Compose


## How to run:

- Before running the docker composer the configurations needs to be fixed.
- Below the technical details of each of the directories are given.
- Read it carefully and make changes according to your need and customize the `docker-compose.yml` file.
- After all the customization run the following command:

```bash
sudo docker-compose -f docker-compose.yml up --build -d
```

- Now all the available services will be live.


## Directory Details:

- **databases:** This directory is used to keep a persistent copy of docker database containers data. Each service container has its own directory here.

- **envs:** This directory holds all the environment variables to run the services. Each service has its separate env files.

- **files:** This directory is used to keep a persistent copy of the static and the media files of the docker coantainers. Each service has their own directory.

- **nginx:** The main Nginx configuration directory. Each of the web based service's respective nginx configs are put in this directory. Here this Nginx is configured to perform only reverse proxy operations. Each service has their own Nginx configured inside there containers.

- **services:** This is where the services code repositories will reside.


<sup> [Pritom Borogoria](https://github.com/saanpritom) reserves all right.</sup>