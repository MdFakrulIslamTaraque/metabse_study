# Installing Metabase in Docker
+ Index
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)


# Prerequisites
- Docker must be installed

# Installation
- Pull the latest Docker image from dockerhub:

```
docker pull metabase/metabase:latest 
```

- Make sure the docker image of metabse `metabase/metabase` is listed after runnig:
```
docker images
```

- Start the Metabase container:
```
docker run -d -p 3000:3000 --name metabase metabase/metabase
```
- Hit the `http://localhost:3000/` to see the metabase UI and setup your metabsae account.

- Optional: to view the logs as your Open Source Metabase initializes, run:

```
docker logs -f metabase
```